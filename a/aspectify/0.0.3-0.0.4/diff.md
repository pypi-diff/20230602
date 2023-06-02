# Comparing `tmp/aspectify-0.0.3.tar.gz` & `tmp/aspectify-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aspectify-0.0.3.tar", last modified: Fri Jun  2 07:29:44 2023, max compression
+gzip compressed data, was "aspectify-0.0.4.tar", last modified: Fri Jun  2 10:53:04 2023, max compression
```

## Comparing `aspectify-0.0.3.tar` & `aspectify-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 07:29:44.120417 aspectify-0.0.3/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-0.0.3/LICENSE
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-0.0.3/MANIFEST.in
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     6872 2023-06-02 07:29:44.120417 aspectify-0.0.3/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     4835 2023-06-02 07:27:18.000000 aspectify-0.0.3/README.md
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 07:29:44.120417 aspectify-0.0.3/aspectify/
--rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-06-02 07:29:39.000000 aspectify-0.0.3/aspectify/__init__.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     1537 2023-06-02 07:29:39.000000 aspectify-0.0.3/aspectify/_modidx.py
--rw-r--r--   0 ruescog   (1008) ruescog   (1011)     6488 2023-06-02 07:29:39.000000 aspectify-0.0.3/aspectify/aop.py
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      142 2023-05-29 07:42:30.000000 aspectify-0.0.3/aspectify/core.py
-drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 07:29:44.120417 aspectify-0.0.3/aspectify.egg-info/
--rw-r-----   0 ruescog   (1008) ruescog   (1011)     6872 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/PKG-INFO
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      361 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/SOURCES.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/dependency_links.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/entry_points.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-0.0.3/aspectify.egg-info/not-zip-safe
--rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/requires.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-06-02 07:29:44.000000 aspectify-0.0.3/aspectify.egg-info/top_level.txt
--rw-r-----   0 ruescog   (1008) ruescog   (1011)      802 2023-06-02 07:29:21.000000 aspectify-0.0.3/settings.ini
--rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-06-02 07:29:44.120417 aspectify-0.0.3/setup.cfg
--rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-0.0.3/setup.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 10:53:04.636672 aspectify-0.0.4/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     7048 2023-05-29 07:08:03.000000 aspectify-0.0.4/LICENSE
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)      111 2023-04-27 10:12:58.000000 aspectify-0.0.4/MANIFEST.in
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4618 2023-06-02 10:53:04.632672 aspectify-0.0.4/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     3109 2023-06-02 10:13:26.000000 aspectify-0.0.4/README.md
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 10:53:04.632672 aspectify-0.0.4/aspectify/
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)       22 2023-06-02 10:53:01.000000 aspectify-0.0.4/aspectify/__init__.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     1537 2023-06-02 10:53:01.000000 aspectify-0.0.4/aspectify/_modidx.py
+-rw-r--r--   0 ruescog   (1008) ruescog   (1011)     5884 2023-06-02 10:53:01.000000 aspectify-0.0.4/aspectify/aop.py
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      142 2023-05-29 07:42:30.000000 aspectify-0.0.4/aspectify/core.py
+drwxr-x---   0 ruescog   (1008) ruescog   (1011)        0 2023-06-02 10:53:04.632672 aspectify-0.0.4/aspectify.egg-info/
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)     4618 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/PKG-INFO
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      361 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/SOURCES.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/dependency_links.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       61 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/entry_points.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        1 2023-05-29 07:48:24.000000 aspectify-0.0.4/aspectify.egg-info/not-zip-safe
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)        7 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/requires.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       10 2023-06-02 10:53:04.000000 aspectify-0.0.4/aspectify.egg-info/top_level.txt
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)      802 2023-06-02 07:38:05.000000 aspectify-0.0.4/settings.ini
+-rw-r-----   0 ruescog   (1008) ruescog   (1011)       38 2023-06-02 10:53:04.636672 aspectify-0.0.4/setup.cfg
+-rw-rw-r--   0 ruescog   (1008) ruescog   (1011)     2596 2023-04-27 10:12:58.000000 aspectify-0.0.4/setup.py
```

### Comparing `aspectify-0.0.3/LICENSE` & `aspectify-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.3/README.md` & `aspectify-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,155 +1,111 @@
-aspectify
-================
-
-<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-
-Aspect Oriented Programming is a programming paradigm that allows the
-user to separate some cross-cutting content from the main code, such as
-the logging or a database connection.
-
-As it may be known, other programming languages has some functionallity
-(implemented or plugged in) to use this paradigm as an additional
-abstract layer to the core application. AspectJ (used in Java), can
-sound familiar to the reader.
-
-In order to bring this amazing and powerful functionality to Python
-(which, in addition, will allow us to add it dynamically instead of
-using a weaver –as it is done in Java–), we have defined `Aspectify`, a
-Python library to manage AOP.
-
-## Background concepts
-
-Before introducing the library, it is important to define some concepts
-used in AOP. Those are: -
-[`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect)
-(*what*): a cross-cutting concept. In fact, an
-[`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect) will
-group some functionalies. These, which will modify the natural behaviour
-of a method, are called `Advice`s. - `PointCut` (*when*): the time at
-which the new behaviuor must occur. Originally, only three points in
-time were defined (`before`, `around` and `after`), but nowadays new
-points in time are defined, such as “after throwing an exception”. -
-`Advice` (*what to do*): as mentioned above, the code fragment to
-execute when the `PointCut` occurs.
-
-## Installation
-
-In order to install the library, it is only needed to execute the pypi
-comand that follows:
-
-``` sh
-pip install aspectify
-```
-
-> **ADVICE**: You should use a virtual environment to install the
-> packages associated with your proyect.
-
-## How to use Aspectify
-
-Once the background is defined and the library installed, we can start
-to create the AOP layer to our projects.
-
-### The core project
-
-In order to use the library, we need a project. For example, here is a
-`Calculator` program, that will apply the basic operators to two values
-entered by keyboard.
-
-``` python
-class Calculator():
-    def __init__(self, a, b):
-        self.a = a
-        self.b = b
-    
-    def add(self):
-        return self.a + self.b
-
-    def subtract(self):
-        return self.a - self.b
-
-    def multiply(self):
-        return self.a * self.b
-
-    def divide(self):
-        return self.a / self.b
-```
-
-Now, we can use it to operate some integers.
-
-``` python
-a = 10
-b = 20
-operator = "+"
-calculator = Calculator(a, b)
-
-if operator == "+":
-    print(calculator.add())
-elif operator == "-":
-    print(calculator.subtract())
-elif operator == "*":
-    print(calculator.multiply())
-elif operator == "/":
-    print(calculator.divide())
-```
-
-    30
-
-A bit rudimentary, but it works.
-
-Now, let us suppose that this `Calculator` program is a library. In
-addition, let us suppose that we did not write it, and we did not have
-the access to they parts: we just know that a `Calculator` class exists
-and it has four methods: `add`, `subtract`, `multiply` and `divide`.
-
-### AOP: definition
-
-At this moment, we want to modify, let us say, the `add` method
-behaviour to add the following message: “Adding some numbers”. We can
-use the library to create an
-[`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect).
-
-> ADVICE: Trying to be as clean as possible, we strongly recomend you to
-> create a **new** `.py` file and add the
-> [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect)s to
-> this file.
-
-First of all, we need to import to the
-[`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect)s file
-(`aspects.py` from now on) the libraries and modules that will be used.
-In this case, the `Calculator`.
-
-``` python
-# aspects.py file
-
-# import Calculator
-from aspectify.aop import Aspect, is_detectable
-```
-
-First of all, we need to define a method to gather all the classes
-loaded in the `aspects.py` file, in order to modify their behaviour
-dynamically. This method will be always be the same:
-
-``` python
-def get_classes():
-    return [element for element in list(globals().items())]
-```
-
-At this point, we can define our first
-[`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect). We will
-call it “add-message”, and it will show a message `before` the addition
-is done.
-
-``` python
-add_message_aspect = Aspect("add-message")
-add_message_aspect.set_before(lambda: print("Adding some numbers"))
-```
-
-Finally, we will create a `PointCut` that will define which methods will
-show this message. We will use the regular expression `.*add`.
-
-``` python
-add_message_aspect.create_pointcut(get_classes(), ".*add")
-```
-
-    Captured method: __main__.Calculator.add
-    [WARNING]: If executed in a notebook, the cell is shown being executed, but this message proves that the execution is finished.
+Metadata-Version: 2.1
+Name: aspectify
+Version: 0.0.4
+Summary: Apply Aspect Oriented Programming to your Python code
+Home-page: https://github.com/ruescog/aspectify
+Author: ruescog
+Author-email: ruescog@unirioja.es
+License: Apache Software License 2.0
+Description: aspectify
+        ================
+        
+        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+        
+        Aspect Oriented Programming is a programming paradigm that allows the
+        user to separate some cross-cutting content from the main code, such as
+        the logging or a database connection.
+        
+        As it may be known, other programming languages has some functionallity
+        (implemented or plugged in) to use this paradigm as an additional
+        abstract layer to the core application.
+        [AspectJ](https://www.eclipse.org/aspectj/) (used in Java), can sound
+        familiar to the reader.
+        
+        In order to bring this amazing and powerful functionality to Python
+        (which, in addition, will allow us to add it dynamically instead of
+        using a weaver –as it is done in Java–), we have defined `Aspectify`, a
+        Python library to manage AOP.
+        
+        ## Background concepts
+        
+        Before introducing the library, it is important to define some concepts
+        used in AOP. Those are: -
+        [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect)
+        (*what*): a cross-cutting concept. In fact, an
+        [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect) will
+        group some functionalies. These, which will modify the natural behaviour
+        of a method, are called `Advice`s. - `PointCut` (*when*): a fragment of
+        code where the
+        [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect) is
+        defined. Can be multiple `PointCut`s for each
+        [`Aspect`](https://ruescog.github.io/aspectify/aop.html#aspect) (indeed,
+        it will). - `Advice` (*when and what to do*): The code fragment to
+        execute when the `PointCut` occurs and the moment when the new behaviuor
+        must occur. Originally, only three moments were defined (`before`,
+        `around` –instead of– and `after`), but nowadays new moments are
+        defined, such as “after throwing an exception” (`after_throwing`) or
+        “after NOT throwing an exception” (`after_returning`).
+        
+        ## Installation
+        
+        In order to install the library, it is only needed to execute the pypi
+        comand that follows:
+        
+        ``` sh
+        pip install aspectify
+        ```
+        
+        > **ADVICE**: You should use a virtual environment to install the
+        > packages associated with your proyect.
+        
+        ## Why do we need Aspectify
+        
+        Once the background is defined and the library is installed, we can
+        start to create the AOP layer to our projects.
+        
+        ### The core project
+        
+        In order to use the library, we need a project. For example, we will use
+        the `random` library for Python.
+        
+        ``` python
+        from random import Random
+        ```
+        
+        Now, we can use it to generate some integers.
+        
+        ``` python
+        r = Random()
+        r.randint(5, 10)
+        ```
+        
+            9
+        
+        As you can see in its documentation, `randint` (called with parameters
+        `a` and `b`) can generate the `b` value itself (it is a closed range
+        \[5, 10\]).
+        
+        If we want to change this behaviour to the normal random functions
+        behaviour (the range is closed-opened \[5, 10)), you will need to
+        redefine it. Furthermore, if other functions or library use this method,
+        they will not use yours.
+        
+        How can we solve it? Using AOP.
+        
+        During this introduction, we have seen the background concepts and how
+        to install the `Aspectify` library. In the next section we will explain
+        how to use it with a simple example.
+        
+Keywords: nbdev jupyter notebook python
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `aspectify-0.0.3/aspectify/_modidx.py` & `aspectify-0.0.4/aspectify/_modidx.py`

 * *Files identical despite different names*

### Comparing `aspectify-0.0.3/aspectify/aop.py` & `aspectify-0.0.4/aspectify/aop.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,45 +2,39 @@
 
 # %% auto 0
 __all__ = ['is_detectable', 'advice', 'Aspect']
 
 # %% ../nbs/00_aop.ipynb 3
 import re
 
+from functools import wraps
+
 # %% ../nbs/00_aop.ipynb 4
-def is_detectable(name, obj):
+def is_detectable(name, # The name of the object.
+                  obj # The builded object (potentially class).
+                 ):
     """
     Determines when an object is potentially detectable to add an aspect to it.
-
-    Params:
-    name: str ; The name of the object.
-    obj: object ; The builded object --generaly a class--.
-
-    Returns:
-    b: boolean ; Whether the `obj` object (so called `name`) is detectable via AOP or not.
-    """
-    return (name not in ["get_ipython", "exit", "quit", "open"]
-            and not isinstance(obj, Aspect)
-            and isinstance(obj, type) # it must be a type (a class)
-            and callable(obj)
+    """
+    return (
+        name not in ["get_ipython", "exit", "quit", "open"]
+        and not isinstance(obj, Aspect)
+        and isinstance(obj, type) # it must be a type (a class)
+        and callable(obj)
             )
 
 # %% ../nbs/00_aop.ipynb 5
-def advice(moment, todo):
+def advice(moment, # One of 'before', 'around', 'after_returning', 'after_throwing' or 'after'. See the documentation for more information.
+           todo # What to do at the selected moment.
+          ):
     """
     Add an advice to a particular function.
-
-    Params:
-    moment: str ; One of 'before', 'around', 'after_returning', 'after_throwing' or 'after'. See the documentation for more information.
-    todo: funtion ; What to do at the selected moment.
-
-    Returns:
-    dec: function ; The modified function.
     """
     def dec(method):
+        @wraps(method)
         def inner(*args, **kwargs):
             todo_args = args[1:] # discards the 0-index argument, which is the object itself
             if moment not in ["before", "around", "after_returning", "after_throwing", "after"]:
                 raise Exception(f"Moment {moment} is not defined.")
 
             try:
                 if moment == "before": todo(*todo_args, **kwargs) # returned value is lost
@@ -56,43 +50,32 @@
     return dec
 
 # %% ../nbs/00_aop.ipynb 6
 class Aspect():
     """
     Defines a complete aspect.
     """
-    def __init__(self, name):
+    def __init__(self):
         """
-        Constructs a new aspect.
-
-        Params:
-        name: str ; The aspect name.
-
-        Returns:
-        None
+        Defines a new aspect.
         """
-        self.name = name
         self.before = None
         self.around = None
         self.after_returning = None
         self.after_throwing = None
         self.after = None
 
     # POINTCUT
-    def create_pointcut(self, objects, pattern, logging = True):
+    def create_pointcut(self,
+                        objects, # All the classes to which the aspect can be added. See the documentation for more information.
+                        pattern, # The pattern (string that defines a regular expression) used to select the methods to be added the aspect.
+                        logging = True # Whether to log the captured methods with the `PointCut`.
+                       ):
         """
         Creates a new pointcut associated with the aspect.
-
-        Params:
-        classes: list ; All the classes to which the aspect can be added. See the documentation for more information.
-        pattern: str ; The pattern (string that defines a regular expression) used to select the methods to be added the aspect.
-        logging: bool = True ; Whether to log the captured methods with the `PointCut`.
-
-        Returns:
-        None
         """
         pattern = re.compile(pattern)
 
         for name, _object in objects:
             if is_detectable(name, _object):
                 for method_name in dir(_object):
                     if "__" in method_name: continue
@@ -115,72 +98,50 @@
                         # saves it
                         try:
                             setattr(_object, method_name, method)
                         except AttributeError as e:
                             if logging: message += "; CANNOT be modified."
                         
                         if logging: print(message)
-        
-        print("[WARNING]: If executed in a notebook, the cell is shown being executed, but this message proves that the execution is finished.")
 
     # ADVICES
-    def set_before(self, function):
+    def set_before(self,
+                   function # The 'to do' function in that moment.
+                  ):
         """
         Determines what to do before the execution of the method.
-
-        Params:
-        function: function ; The 'to do' function in that moment.
-
-        Returns:
-        None
         """
         self.before = function
     
-    def set_around(self, function):
+    def set_around(self,
+                   function # The 'to do' function in that moment.
+                  ):
         """
         Determines what to do instead of the execution of the method.
-
-        Params:
-        function: function ; The 'to do' function in that moment.
-
-        Returns:
-        None
         """
         self.around = function
     
-    def set_after_returning(self, function):
+    def set_after_returning(self,
+                            function # The 'to do' function in that moment.
+                           ):
         """
         Determines what to do after a complete execution of the method (when there are not exceptions).
-
-        Params:
-        function: function ; The 'to do' function in that moment.
-
-        Returns:
-        None
         """
         self.after_returning = function
     
-    def set_after_throwing(self, function):
+    def set_after_throwing(self,
+                           function # The 'to do' function in that moment.
+                          ):
         """
         Determines what to do when the execution of the method raises an exception.
         
         * BEWARE! This method will not handle the exception (it will be finally raised), but it will allow you to do something when the exception is raised.
-
-        Params:
-        function: function ; The 'to do' function in that moment.
-
-        Returns:
-        None
         """
         self.after_throwing = function
 
-    def set_after(self, function):
+    def set_after(self,
+                  function # The 'to do' function in that moment.
+                 ):
         """
         Determines what to do after the execution of the method. This function will be always executed after the `after_returning` and `after_throwing` functions.
-        
-        Params:
-        function: function ; The 'to do' function in that moment.
-
-        Returns:
-        None
         """
         self.after = function
```

### Comparing `aspectify-0.0.3/settings.ini` & `aspectify-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = aspectify
 lib_name = aspectify
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = aspectify
 nbs_path = nbs
 recursive = True
```

### Comparing `aspectify-0.0.3/setup.py` & `aspectify-0.0.4/setup.py`

 * *Files identical despite different names*

