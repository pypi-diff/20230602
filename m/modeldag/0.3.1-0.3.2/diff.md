# Comparing `tmp/modeldag-0.3.1.tar.gz` & `tmp/modeldag-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modeldag-0.3.1.tar", last modified: Fri Jun  2 08:41:55 2023, max compression
+gzip compressed data, was "modeldag-0.3.2.tar", last modified: Fri Jun  2 09:18:10 2023, max compression
```

## Comparing `modeldag-0.3.1.tar` & `modeldag-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 08:41:55.737648 modeldag-0.3.1/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.3.1/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 08:41:55.737722 modeldag-0.3.1/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     1896 2023-06-02 08:39:03.000000 modeldag-0.3.1/README.md
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 08:41:55.736869 modeldag-0.3.1/modeldag/
--rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-06-02 08:41:36.000000 modeldag-0.3.1/modeldag/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    14472 2023-06-02 08:41:09.000000 modeldag-0.3.1/modeldag/modeldag.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 08:41:55.737553 modeldag-0.3.1/modeldag.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.3.1/modeldag.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/top_level.txt
--rw-r--r--   0 rigault   (2358) staff       (20)     1020 2023-06-02 08:41:55.738034 modeldag-0.3.1/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.3.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 09:18:10.174135 modeldag-0.3.2/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.3.2/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 09:18:10.174199 modeldag-0.3.2/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     1896 2023-06-02 08:39:03.000000 modeldag-0.3.2/README.md
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 09:18:10.173397 modeldag-0.3.2/modeldag/
+-rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-06-02 09:18:01.000000 modeldag-0.3.2/modeldag/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    14448 2023-06-02 09:10:36.000000 modeldag-0.3.2/modeldag/modeldag.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 09:18:10.174044 modeldag-0.3.2/modeldag.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.3.2/modeldag.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-06-02 09:18:10.000000 modeldag-0.3.2/modeldag.egg-info/top_level.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)     1020 2023-06-02 09:18:10.174517 modeldag-0.3.2/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.3.2/setup.py
```

### Comparing `modeldag-0.3.1/LICENSE` & `modeldag-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modeldag-0.3.1/PKG-INFO` & `modeldag-0.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.3.1
+Version: 0.3.2
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `modeldag-0.3.1/README.md` & `modeldag-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `modeldag-0.3.1/modeldag/modeldag.py` & `modeldag-0.3.2/modeldag/modeldag.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,31 +120,31 @@
         """ get a copy of the model 
         
         Parameters
         ----------
 
         **kwargs can change the model entry parameters
             for istance, t0: {"low":0, "high":10}
-            will update model["t0"]["param"] = ...
+            will update model["t0"]["kwargs"] = ...
 
         Returns
         -------
         dict
            a copy of the model (with param potentially updated)
         """
         model = deepcopy(self.model)
         for k,v in kwargs.items():
-            model[k]["param"].update(v)
+            model[k]["kwargs"].update(v)
 
         return model
     
     def change_model(self, **kwargs):
         """ change the model attached to this instance
         
-        **kwargs will update the entry  parameters ("param", e.g. t0["param"])
+        **kwargs will update the entry  parameters ("param", e.g. t0["kwargs"])
 
         See also
         --------
         get_model: get a copy of the model
         """
         self.model = self.get_model(**kwargs)
 
@@ -305,46 +305,46 @@
 
         Parameters
         ----------
         name: str
             name of the variable
             
         func: str, function
-            what model should be used to draw the parameter
+            what func should be used to draw the parameter
 
         size: int
             number of line to be draw
 
         xx: str, array
-           provide this *if* the model_func returns the pdf and not sampling.
+           provide this *if* the func returns the pdf and not sampling.
            xx defines where the pdf will be evaluated.
            if xx is a string, it will be assumed to be a np.r_ entry (``np.r_[xx]``)
 
         Returns
         -------
         list 
             
         """
         # Flexible origin of the sampling method
-        func = self._parse_inputmodel_func(name=name, func=func)
+        func = self._parse_input_func(name=name, func=func)
         
         # Check the function parameters
         try:
             func_arguments = list(inspect.getfullargspec(func).args)
         except: # fail for Cython functions
-            #warnings.warn(f"inspect failed for {name}{model} -> {func}")
+            #warnings.warn(f"inspect failed for {name}{func} -> {func}")
             func_arguments = ["size"] # let's assume this as for numpy.random or scipy.
 
         # And set the correct parameters
         prop = {}
         if "size" in func_arguments:
             prop["size"] = size
             
-        if "model" in func_arguments and model is not None: # means you left the default
-            prop["func"] = model
+        if "func" in func_arguments and func is not None: # means you left the default
+            prop["func"] = func
 
         if "xx" in func_arguments and xx is not None: # if xx is None
             if type(xx) == str: # assumed r_ input
                 xx = eval(f"np.r_[{xx}]")
                 
             prop["xx"] = xx
 
@@ -411,27 +411,27 @@
             output_name = param_model.get("as", param_name)
             if output_name is None: # solves 'as' = None case.
                 output_name = param_name
             data[output_name] = samples.T
 
         return data
     
-    def _parse_inputmodel_func(self, name=None, func=None):
-        """ returns the function associated to the input model.
+    def _parse_input_func(self, name=None, func=None):
+        """ returns the function associated to the input func.
 
         """
-        if callable(func): # model is a function. Good to go.
+        if callable(func): # func is a function. Good to go.
             return func
         
-        # model is a method of this instance ?
-        if model is not None and hasattr(self, func):
+        # func is a method of this instance ?
+        if func is not None and hasattr(self, func):
             func = getattr(self, func)
             
-        # model is a method a given object ?
-        elif model is not None and hasattr(self.obj, func):
+        # func is a method a given object ?
+        elif func is not None and hasattr(self.obj, func):
             func = getattr(self.obj, func)
             
         # name is a draw_ method of this instance object ?            
         elif hasattr(self, f"draw_{name}"):
             func = getattr(self,f"draw_{name}")
 
         # name is a draw_ method of this instance object ?
```

### Comparing `modeldag-0.3.1/modeldag.egg-info/PKG-INFO` & `modeldag-0.3.2/modeldag.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.3.1
+Version: 0.3.2
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `modeldag-0.3.1/setup.cfg` & `modeldag-0.3.2/setup.cfg`

 * *Files identical despite different names*

