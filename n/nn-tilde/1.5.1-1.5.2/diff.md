# Comparing `tmp/nn_tilde-1.5.1.tar.gz` & `tmp/nn_tilde-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_tilde-1.5.1.tar", last modified: Tue May 30 13:55:08 2023, max compression
+gzip compressed data, was "nn_tilde-1.5.2.tar", last modified: Fri Jun  2 15:55:06 2023, max compression
```

## Comparing `nn_tilde-1.5.1.tar` & `nn_tilde-1.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:55:08.653288 nn_tilde-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-05-30 13:53:17.000000 nn_tilde-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 13:53:17.000000 nn_tilde-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-30 13:55:08.653288 nn_tilde-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-05-30 13:53:17.000000 nn_tilde-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:55:08.653288 nn_tilde-1.5.1/nn_tilde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-30 13:55:08.000000 nn_tilde-1.5.1/nn_tilde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-30 13:55:08.000000 nn_tilde-1.5.1/nn_tilde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:55:08.000000 nn_tilde-1.5.1/nn_tilde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 13:55:08.000000 nn_tilde-1.5.1/nn_tilde.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 13:55:08.000000 nn_tilde-1.5.1/nn_tilde.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:55:08.653288 nn_tilde-1.5.1/python_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-30 13:53:17.000000 nn_tilde-1.5.1/python_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 13:53:17.000000 nn_tilde-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:55:08.653288 nn_tilde-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-30 13:53:17.000000 nn_tilde-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:55:06.826599 nn_tilde-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-02 15:55:06.826599 nn_tilde-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:55:06.822599 nn_tilde-1.5.2/nn_tilde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 15:55:06.000000 nn_tilde-1.5.2/nn_tilde.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:55:06.822599 nn_tilde-1.5.2/python_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/python_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:55:06.826599 nn_tilde-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-02 15:53:02.000000 nn_tilde-1.5.2/setup.py
```

### Comparing `nn_tilde-1.5.1/LICENSE` & `nn_tilde-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.1/PKG-INFO` & `nn_tilde-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn_tilde
-Version: 1.5.1
+Version: 1.5.2
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.1 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn_tilde Version: 1.5.2 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
```

### Comparing `nn_tilde-1.5.1/README.md` & `nn_tilde-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nn_tilde-1.5.1/nn_tilde.egg-info/PKG-INFO` & `nn_tilde-1.5.2/nn_tilde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn-tilde
-Version: 1.5.1
+Version: 1.5.2
 Summary: Set of tools to create nn_tilde compatible models.
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.1 Summary: Set of tools to
+Metadata-Version: 2.1 Name: nn-tilde Version: 1.5.2 Summary: Set of tools to
 create nn_tilde compatible models. Author: Antoine CAILLON Author-email:
 caillon@ircam.fr Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE ![banner](https://github.com/acids-ircam/nn_tilde/raw/
 master/assets/banner.png) # Demonstration video [![RAVE x nn~](http://
 img.youtube.com/vi/dMZs04TzxUI/mqdefault.jpg)](https://www.youtube.com/
```

### Comparing `nn_tilde-1.5.1/python_tools/__init__.py` & `nn_tilde-1.5.2/python_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import inspect
 import logging
-from typing import Any, Callable, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, List, Optional, Sequence, Tuple, Union
 
 import cached_conv as cc
 import torch
 
 TYPE_HASH = {bool: 0, int: 1, float: 2, str: 3, torch.Tensor: 4}
 
 
 class Module(torch.nn.Module):
 
     def __init__(self) -> None:
         super().__init__()
         self._methods = []
-        self._attributes = []
+        self._attributes = ["none"]
 
     def register_method(
         self,
         method_name: str,
         in_channels: int,
         in_ratio: int,
         out_channels: int,
@@ -115,15 +115,15 @@
                         (f"Wrong output length for method \"{method_name}\", "
                          f"expected {test_buffer_size//out_ratio} "
                          f"got {y.shape[2]}"))
                 logging.info((f"Added method \"{method_name}\" "
                               f"tested with buffer size {test_buffer_size}"))
             else:
                 logging.info(
-                    f"Skiping method {method_name} with mc.nn~ API as cc.MAX_BATCH_SIZE={cc.MAX_BATCH_SIZE}"
+                    f"Skipping method {method_name} with mc.nn~ API as cc.MAX_BATCH_SIZE={cc.MAX_BATCH_SIZE}"
                 )
         else:
             logging.warn(f"Added method \"{method_name}\" without testing it.")
 
         self._methods.append(method_name)
 
     def register_attribute(self, attribute_name: str,
@@ -146,25 +146,24 @@
             raise AttributeError(f"Setter for {attribute_name} not defined")
 
         signature = inspect.signature(getattr(self, f"get_{attribute_name}"))
         if signature.return_annotation == inspect._empty:
             raise TypeError(
                 f"Output type not defined for getter get_{attribute_name}")
 
-        # self.register_buffer(attribute_name, torch.Tensor(values))
         self.__setattr__(attribute_name, values)
         self.register_buffer(f"{attribute_name}_params",
                              torch.Tensor(type_hash))
         self._attributes.append(attribute_name)
 
     @torch.jit.export
     def get_methods(self):
         return self._methods
 
     @torch.jit.export
-    def get_attributes(self):
+    def get_attributes(self) -> List[str]:
         return self._attributes
 
     def export_to_ts(self, path):
         self.eval()
         scripted = torch.jit.script(self)
         scripted.save(path)
```

### Comparing `nn_tilde-1.5.1/setup.py` & `nn_tilde-1.5.2/setup.py`

 * *Files identical despite different names*

