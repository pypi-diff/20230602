# Comparing `tmp/modeldag-0.2.0.tar.gz` & `tmp/modeldag-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modeldag-0.2.0.tar", last modified: Thu Jun  1 14:43:31 2023, max compression
+gzip compressed data, was "modeldag-0.3.1.tar", last modified: Fri Jun  2 08:41:55 2023, max compression
```

## Comparing `modeldag-0.2.0.tar` & `modeldag-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-01 14:43:31.855946 modeldag-0.2.0/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.2.0/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-01 14:43:31.856007 modeldag-0.2.0/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)       88 2023-05-31 13:06:56.000000 modeldag-0.2.0/README.md
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-01 14:43:31.855151 modeldag-0.2.0/modeldag/
--rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-06-01 14:40:56.000000 modeldag-0.2.0/modeldag/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    14379 2023-06-01 13:08:11.000000 modeldag-0.2.0/modeldag/modeldag.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-01 14:43:31.855859 modeldag-0.2.0/modeldag.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-01 14:43:31.000000 modeldag-0.2.0/modeldag.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-06-01 14:43:31.000000 modeldag-0.2.0/modeldag.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-01 14:43:31.000000 modeldag-0.2.0/modeldag.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.2.0/modeldag.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-06-01 14:43:31.000000 modeldag-0.2.0/modeldag.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-06-01 14:43:31.000000 modeldag-0.2.0/modeldag.egg-info/top_level.txt
--rw-r--r--   0 rigault   (2358) staff       (20)     1020 2023-06-01 14:43:31.856315 modeldag-0.2.0/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.2.0/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 08:41:55.737648 modeldag-0.3.1/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2023-05-31 13:06:56.000000 modeldag-0.3.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 08:41:55.737722 modeldag-0.3.1/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     1896 2023-06-02 08:39:03.000000 modeldag-0.3.1/README.md
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 08:41:55.736869 modeldag-0.3.1/modeldag/
+-rw-r--r--   0 rigault   (2358) staff       (20)       47 2023-06-02 08:41:36.000000 modeldag-0.3.1/modeldag/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    14472 2023-06-02 08:41:09.000000 modeldag-0.3.1/modeldag/modeldag.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-06-02 08:41:55.737553 modeldag-0.3.1/modeldag.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      741 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      268 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 13:38:23.000000 modeldag-0.3.1/modeldag.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)       55 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        9 2023-06-02 08:41:55.000000 modeldag-0.3.1/modeldag.egg-info/top_level.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)     1020 2023-06-02 08:41:55.738034 modeldag-0.3.1/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2023-05-31 13:36:34.000000 modeldag-0.3.1/setup.py
```

### Comparing `modeldag-0.2.0/LICENSE` & `modeldag-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modeldag-0.2.0/PKG-INFO` & `modeldag-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.2.0
+Version: 0.3.1
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `modeldag-0.2.0/modeldag/modeldag.py` & `modeldag-0.3.1/modeldag/modeldag.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,33 @@
 
 #__all__ = ["ModelDAG"]
 
 def modeldict_to_modeldf(model):
     """ """
     dd = pandas.DataFrame(list(model.values()), 
                           index=model.keys()).reset_index(names=["model_name"])
-    # naming convention
-    f_ = dd["as"].fillna(dict(dd["model_name"]))
-    f_.name = "entry"
-    # merge and explode the names and inputs
-    return dd.join(f_)
+    if "as" not in dd:
+        dd["as"] = dd["model_name"]
+        dd["entry"] = dd["as"]
+    else:
+        # naming convention
+        f_ = dd["as"].fillna( dict(dd["model_name"]) )
+        f_.name = "entry"
+        dd = dd.join(f_) # merge and explode the names and inputs
+        
+    return dd
 
 
 class ModelDAG( object ):
     """
     Models are dict of arguments that may have 3 entries:
-    {
-    "element_1":{model:func, kwargs: dict, as: str_or_list},
-    "element_2":{model:func, param: dict, as: str_or_list},
-    "element_3":{model:func, param: dict, as: str_or_list},
-    ...
-    }
+    model = {key1 : {'func': func, 'kwargs': dict, 'as': None_str_list'},
+             key2 : {'func': func, 'kwargs': dict, 'as': None_str_list'},
+             ...
+             }
     
     """
     def __init__(self, model={}, obj=None):
         """ 
         
         Parameters
         ----------
@@ -293,23 +296,23 @@
         pandas.DataFrame
             N=size lines and at least 1 column per model entry
         """
         model = self.get_model(**kwargs)
         return self._draw(model, size=size, limit_to_entries=limit_to_entries,
                               data=data)
     
-    def draw_param(self, name=None, model=None, size=None, xx=None, **kwargs):
+    def draw_param(self, name=None, func=None, size=None, xx=None, **kwargs):
         """ draw a single entry of the model
 
         Parameters
         ----------
         name: str
             name of the variable
             
-        model_func: str, function
+        func: str, function
             what model should be used to draw the parameter
 
         size: int
             number of line to be draw
 
         xx: str, array
            provide this *if* the model_func returns the pdf and not sampling.
@@ -318,30 +321,30 @@
 
         Returns
         -------
         list 
             
         """
         # Flexible origin of the sampling method
-        func = self._parse_inputmodel_func(name=name, model=model)
+        func = self._parse_inputmodel_func(name=name, func=func)
         
         # Check the function parameters
         try:
             func_arguments = list(inspect.getfullargspec(func).args)
         except: # fail for Cython functions
             #warnings.warn(f"inspect failed for {name}{model} -> {func}")
             func_arguments = ["size"] # let's assume this as for numpy.random or scipy.
 
         # And set the correct parameters
         prop = {}
         if "size" in func_arguments:
             prop["size"] = size
             
         if "model" in func_arguments and model is not None: # means you left the default
-            prop["model"] = model
+            prop["func"] = model
 
         if "xx" in func_arguments and xx is not None: # if xx is None
             if type(xx) == str: # assumed r_ input
                 xx = eval(f"np.r_[{xx}]")
                 
             prop["xx"] = xx
 
@@ -391,15 +394,15 @@
             for k, v in inprop.items():
                 if type(v) is str and "@" in v:
                     key = v.split("@")[-1].split(" ")[0]
                     inprop[k] = data[key].values
                     params["size"] = None
                     
             # set the model ; this overwrite prop['model'] but that make sense.
-            inprop["model"] = param_model.get("model", None)
+            inprop["func"] = param_model.get("func", None)
             
             # update the general properties for that of this parameters
             prop = {**params, **inprop}
 
             # 
             # Draw it
             samples = np.asarray(self.draw_param(param_name, **prop))
@@ -408,42 +411,42 @@
             output_name = param_model.get("as", param_name)
             if output_name is None: # solves 'as' = None case.
                 output_name = param_name
             data[output_name] = samples.T
 
         return data
     
-    def _parse_inputmodel_func(self, name=None, model=None):
+    def _parse_inputmodel_func(self, name=None, func=None):
         """ returns the function associated to the input model.
 
         """
-        if callable(model): # model is a function. Good to go.
-            return model
+        if callable(func): # model is a function. Good to go.
+            return func
         
         # model is a method of this instance ?
-        if model is not None and hasattr(self, model):
-            func = getattr(self, model)
+        if model is not None and hasattr(self, func):
+            func = getattr(self, func)
             
         # model is a method a given object ?
-        elif model is not None and hasattr(self.obj, model):
-            func = getattr(self.obj, model)
+        elif model is not None and hasattr(self.obj, func):
+            func = getattr(self.obj, func)
             
         # name is a draw_ method of this instance object ?            
         elif hasattr(self, f"draw_{name}"):
             func = getattr(self,f"draw_{name}")
 
         # name is a draw_ method of this instance object ?            
         elif hasattr(self.obj, f"draw_{name}"):
             func = getattr(self.obj, f"draw_{name}")
         
         else:
             try:
-                func = eval(model) # if you input a string of a function known by python somehow ?
+                func = eval(func) # if you input a string of a function known by python somehow ?
             except:
-                raise ValueError(f"Cannot parse the input function {name}:{model}")
+                raise ValueError(f"Cannot parse the input function {name}:{func}")
         
         return func
 
     # =================== #
     #   Properties        #
     # =================== #
     @property
```

### Comparing `modeldag-0.2.0/modeldag.egg-info/PKG-INFO` & `modeldag-0.3.1/modeldag.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modeldag
-Version: 0.2.0
+Version: 0.3.1
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/modeldag
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: BSD 3-Clause "New" or "Revised" License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `modeldag-0.2.0/setup.cfg` & `modeldag-0.3.1/setup.cfg`

 * *Files identical despite different names*

