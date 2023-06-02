# Comparing `tmp/langdash-0.0.4.dev2.tar.gz` & `tmp/langdash-0.0.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.4.dev2.tar", last modified: Wed May 31 21:54:53 2023, max compression
+gzip compressed data, was "langdash-0.0.5.dev1.tar", last modified: Fri Jun  2 02:00:55 2023, max compression
```

## Comparing `langdash-0.0.4.dev2.tar` & `langdash-0.0.5.dev1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.4.dev2/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.4.dev2/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3575 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2690 2023-05-31 21:54:27.000000 langdash-0.0.4.dev2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-05-31 21:53:10.000000 langdash-0.0.4.dev2/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    17611 2023-05-31 19:50:04.000000 langdash-0.0.4.dev2/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.484769 langdash-0.0.4.dev2/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.4.dev2/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.4.dev2/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     4126 2023-05-31 20:08:59.000000 langdash-0.0.4.dev2/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      690 2023-05-31 17:39:51.000000 langdash-0.0.4.dev2/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-05-31 17:04:37.000000 langdash-0.0.4.dev2/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7520 2023-05-31 19:52:12.000000 langdash-0.0.4.dev2/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.484769 langdash-0.0.4.dev2/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.4.dev2/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.4.dev2/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7041 2023-05-31 20:11:04.000000 langdash-0.0.4.dev2/langdash/models/rwkvcpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      958 2023-05-31 20:11:54.000000 langdash-0.0.4.dev2/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6134 2023-05-31 20:11:31.000000 langdash-0.0.4.dev2/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      835 2023-05-31 17:40:54.000000 langdash-0.0.4.dev2/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2436 2023-05-31 17:34:53.000000 langdash-0.0.4.dev2/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.4.dev2/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.4.dev2/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.4.dev2/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.4.dev2/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3575 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1214 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 21:54:53.000000 langdash-0.0.4.dev2/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 21:54:53.488764 langdash-0.0.4.dev2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1474 2023-05-31 21:52:17.000000 langdash-0.0.4.dev2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.5.dev1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.5.dev1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3600 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2690 2023-05-31 21:54:27.000000 langdash-0.0.5.dev1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       66 2023-06-02 01:58:48.000000 langdash-0.0.5.dev1/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18804 2023-06-02 01:08:06.000000 langdash-0.0.5.dev1/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.262499 langdash-0.0.5.dev1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.5.dev1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.5.dev1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4314 2023-06-01 22:52:48.000000 langdash-0.0.5.dev1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      690 2023-05-31 17:39:51.000000 langdash-0.0.5.dev1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-05-31 17:04:37.000000 langdash-0.0.5.dev1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7535 2023-06-02 01:14:27.000000 langdash-0.0.5.dev1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.5.dev1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4698 2023-06-01 18:29:41.000000 langdash-0.0.5.dev1/langdash/models/llamacpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.5.dev1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7462 2023-06-02 01:18:48.000000 langdash-0.0.5.dev1/langdash/models/rwkvcpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      958 2023-05-31 20:11:54.000000 langdash-0.0.5.dev1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6250 2023-06-02 01:19:21.000000 langdash-0.0.5.dev1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      835 2023-05-31 17:40:54.000000 langdash-0.0.5.dev1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2598 2023-06-02 00:56:32.000000 langdash-0.0.5.dev1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.5.dev1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.5.dev1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.5.dev1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.5.dev1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3600 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1242 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      161 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-02 02:00:55.000000 langdash-0.0.5.dev1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-02 02:00:55.266499 langdash-0.0.5.dev1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1522 2023-06-01 18:02:29.000000 langdash-0.0.5.dev1/setup.py
```

### Comparing `langdash-0.0.4.dev2/LICENSE.txt` & `langdash-0.0.5.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/PKG-INFO` & `langdash-0.0.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.4.dev2
+Version: 0.0.5.dev1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: embeddings
 Provides-Extra: rwkvcpp
+Provides-Extra: llamacpp
 Provides-Extra: transformers
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
 A simple library for interfacing with language models.
```

### Comparing `langdash-0.0.4.dev2/README.md` & `langdash-0.0.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/chains.py` & `langdash-0.0.5.dev1/langdash/chains.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from collections import OrderedDict
 from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, TYPE_CHECKING
 import re
 import random
+import copy
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
 from langdash.infer import InferArgs
 
 if TYPE_CHECKING:
   from langdash._langdash import Langdash
   from langdash.llm_session import LLMGenerationSession, LLMState
@@ -202,14 +203,22 @@
     return self._call(session=self._load_session(ctx), **kwargs)
 
 @dataclass
 class LDChainCacheState:
   state: "LLMState"
   skip_nodes: int
 
+LDChainCacheStoreDict = OrderedDict[FrozenSet[Tuple[str, Any]], LDChainCacheState]
+
+@dataclass(frozen=True)
+class LDChainCacheStore:
+  _dict: LDChainCacheStoreDict
+  _model: str
+  _model_kwargs: dict
+
 class LDChainCached(LDChain):
   
   def __init__(self, model: str, model_kwargs: dict, **kwargs):
     for k, v in kwargs.items():
       setattr(self, k, v)
       
     self._model = model
@@ -230,21 +239,46 @@
         _arg_first_used_at[k] = self._any_arg_first_use
     
     self._arg_first_used_at: Dict[str, int] = _arg_first_used_at
     self._arg_first_used_at_ordered: List[str] = list(_arg_first_used_at.keys())
     self._arg_first_used_at_ordered.sort(key=lambda k: _arg_first_used_at[k])
     
     # cache session per argument use
-    self._state_cache: OrderedDict[FrozenSet[Tuple[str, Any]], LDChainCacheState] = OrderedDict()
+    self._state_cache: LDChainCacheStoreDict = OrderedDict()
     if len(self._args) == 0:
       self.max_states_to_cache = 1
     else:
       self.max_states_to_cache = min(len(self._args) + 2, 8)
     self._skip_nodes = 0
   
+  # State cache functions
+  
+  def load_cache_store(self, cache_store: LDChainCacheStore):
+    """
+    Loads the cache store from previous inference time.
+    Raises `ValueError` if the model names mismatch.
+    This function expects that the model data of the parent Langdash instance does not change across session. If it does, a `UserWarning` is raised.
+    
+    Args:
+      cache_store (LDChainCacheStore): The cache store.
+    """
+    if self._model != cache_store._model:
+      raise ValueError("model mismatch for LDChainCacheStore")
+    if self._model_kwargs != cache_store._model_kwargs:
+      raise UserWarning("model kwargs does not match LDChainCacheStore, unexpected behavior might occur")
+    self._state_cache = cache_store._dict
+  
+  def save_cache_store(self) -> LDChainCacheStore:
+    """ Saves the cache store into an object. """
+    return LDChainCacheStore(
+      _dict=copy.deepcopy(self._state_cache),
+      _model=self._model,
+      _model_kwargs=copy.deepcopy(self._model_kwargs)
+    )
+  
   def _set_state_cache(
     self,
     key: FrozenSet[Tuple[str, Any]],
     value: LDChainCacheState):
     self._state_cache[key] = value
     self._update_state_cache(key)
     if len(self._state_cache) > self.max_states_to_cache:
@@ -252,14 +286,23 @@
   
   def _update_state_cache(self, key: FrozenSet[Tuple[str, Any]]):
     self._state_cache.move_to_end(key, last=False)
   
   def _get_state_cache(self, key: FrozenSet[Tuple[str, Any]]) -> LDChainCacheState:
     self._update_state_cache(key)
     return self._state_cache[key]
+      
+  def _arg_subset_sorted_by_idx(self, args: LDNodeArgs):
+    current_subset: LDNodeArgs = {}
+    yield current_subset
+    for arg in self._arg_first_used_at_ordered:
+      current_subset[arg] = args[arg]
+      yield current_subset
+  
+  # Inference functions
   
   def _node_pass(self, session: "LLMGenerationSession", args: LDNodeArgs):
     last_state_key: Optional[LDChainCacheState] = None
     for i in range(self._skip_nodes, len(self._nodes)):
       node = self._nodes[i]
       session.tokens_counter = 0
       yield node
@@ -289,21 +332,14 @@
         last_state_key = self._state_cache[current_keys]
       else:
         last_state_key = None
       session._append_called_chain(node, args, session.tokens_counter)
 
   def _create_new_session(self) -> "LLMGenerationSession":
     return self._ld.session_for_model(self._model, **self._model_kwargs)
-      
-  def _arg_subset_sorted_by_idx(self, args: LDNodeArgs):
-    current_subset: LDNodeArgs = {}
-    yield current_subset
-    for arg in self._arg_first_used_at_ordered:
-      current_subset[arg] = args[arg]
-      yield current_subset
 
   def _load_session(
     self,
     args: Optional[LDNodeArgs] = None) -> "LLMGenerationSession":
     session = self._create_new_session()
     
     if frozenset() not in self._state_cache:
@@ -455,29 +491,29 @@
   
 class LDReturns(LDNode):
   """ Return node """
   
   def __init__(self, ld: "Langdash",
                returns: str,
                end: Optional[Union[str, int]],
-               padleft: Optional[str] = None,
+               padleft: str = "",
                inference_args: Optional[InferArgs] = None):
     super().__init__(ld)
     self._returns = returns
     self._end = end
     self._padleft = padleft
     self._inference_args = inference_args
   
   def __repr__(self):
     return f"<Returns arg={self._returns}>"
   
   def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
     for i, respinfer in enumerate(session.infer(end=self._end, args=self._inference_args)):
       if i == 0:
-        if self._padleft is not None and respinfer.tokstr.startswith(self._padleft):
+        if self._padleft and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       yield respinfer
       
 class LDChoice(LDNode):
   """ Choice node """
   
   def __init__(self, ld: "Langdash",
```

### Comparing `langdash-0.0.4.dev2/langdash/classify/token_qa.py` & `langdash-0.0.5.dev1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/core.py` & `langdash-0.0.5.dev1/langdash/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,78 +71,79 @@
     return LDChain(self, *args, **kwargs)
     
   def text(self, *args, **kwargs):
     """
     Creates a raw text node.
     
     Args:
-      text: The raw text.
+      text (str): The raw text.
       
     Returns:
       The text node.
     """
     return LDText(self, *args, **kwargs)
     
   def format_args(self, *args, **kwargs):
     """
     Creates a format argument node.
     
     Args:
-      text: The format text.
+      text (str): The format text.
       
     Returns:
       The format text node.
     """
     return LDFormatArg(self, *args, **kwargs)
     
   def arg(self, *args, **kwargs):
     """
     Creates a new argument node with the specified argument.
     
     Args:
-      arg: The argument.
-      padleft:
+      arg (str): The argument.
+      padleft (str):
         The padding string to use for the left side of the argument.
-      padright:
+      padright (str):
         The padding string to use for the right side of the argument.
     
     Returns:
       The newly created argument node.
     """
     return LDArg(self, *args, **kwargs)
     
   def returns(self, *args, **kwargs):
     """
     Create a new return node for the specified return value.
 
     Args:
-      returns: The name of the return value.
-      end:
+      returns (str): The name of the return value.
+      end (str):
         Where to stop the inference. Either a string, or a token id.
         If None is passed, the inference will continue forever (for streaming).
-      padleft:
-        The padding value for the return.
-      inference_args:
-        The inference arguments for the function.
+      padleft (str):
+        The left padding value for the return. If the generated string starts with
+        *padleft* then it will be stripped.
+      inference_args (Optional[InferArgs]):
+        Optional inference arguments for generation.
 
     Returns:
       The return node.
     """
     return LDReturns(self, *args, **kwargs)
 
   def choice(self, *args, **kwargs):
     """
     Creates a new choice node with the specified choices, and returns to the .
     
     Args:
-      returns: The name of the return value.
-      choices: List of choice strings
-      padleft:
+      returns (str): The name of the return value.
+      choices (List[str]): List of choice strings
+      padleft (str):
         Left padding for every choice string.
-      padright:
+      padright (str):
         Right padding for every choice string.
     
     Returns:
       The newly created choice node.
     """
     return LDChoice(self, *args, **kwargs)
```

### Comparing `langdash-0.0.4.dev2/langdash/infer.py` & `langdash-0.0.5.dev1/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/llm.py` & `langdash-0.0.5.dev1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/llm_session.py` & `langdash-0.0.5.dev1/langdash/llm_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import TypeVar, Generic, Optional, List, Generator, Union, Tuple, TYPE_CHECKING
-from collections.abc import Sequence
 import copy
 
 from langdash.response import RespInfer
 from langdash.chains import CalledChain, LDNodeArgs, LDNode
 from langdash.infer import InferArgs
 from langdash.llm import LLM
 
@@ -105,17 +104,18 @@
   
   def next_token_probs(self) -> List[float]:
     """
     Returns the probabilities for next token.
     """
     raise NotImplementedError("next_token_probs")
   
-  def _infer(self,
-            end: Optional[Union[str, int]],
-            args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
+  def _infer(
+    self,
+    end: Optional[Union[str, int]],
+    args: InferArgs) -> Generator[RespInfer, None, None]:
     raise NotImplementedError("_infer")
 
   def infer(self,
             end: Optional[Union[str, int]],
             args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
     """
     Infer the next token from the input sequence.
@@ -144,14 +144,20 @@
   
   _logits: Optional[T_Logits]
   _next_token: Optional[Tuple[int, str]]
   
   def _eval(self, tokid: int) -> T_Logits:
     raise NotImplementedError("_eval")
   
+  def _eval_mult(self, tokens: List[int]):
+    assert tokens, "tokens must not be empty"
+    for tokid in tokens:
+      logits = self._eval(tokid)
+    return logits
+  
   def _next_token_probs(self):
     raise NotImplementedError("_next_token_probs")
   
   def flush_token(self):
     """
     Flushes the previous token into the language model if healing is enabled.
     
@@ -166,56 +172,53 @@
   def next_token_probs(self, *args, **kwargs) -> List[float]:
     assert self._next_token is None, "token healing must be disabled or flush_token() must be called"
     probs = self._next_token_probs(*args, **kwargs)
     return list(map(float, probs))
   
   def inject(self, text: Union[str, int], add_special_tokens: bool = False) -> int:
     if isinstance(text, str):
-      input_ids = self.tokenize(text, add_special_tokens=add_special_tokens)
+      tokens = self.tokenize(text, add_special_tokens=add_special_tokens)
     else:
-      input_ids = [text]
-    if not input_ids:
+      tokens = [text]
+    if not tokens:
       return 0
     
     num_toks = 0
       
     if self.token_healing:
       init_offset = 0
       if self._next_token is not None:
         tokid, tokstr = self._next_token
-        healed_str = self.decode([tokid, input_ids[0]])
+        healed_str = self.decode([tokid, tokens[0]])
         healed_tokens = self.tokenize(healed_str, add_special_tokens=add_special_tokens)
         
-        if len(input_ids) == 1:
+        if len(tokens) == 1:
           if len(healed_tokens) == 1:
             self._next_token = (healed_tokens[0], healed_str)
             return 1
           else:
             # handle rare case where 1 input token maps to 2 or more "healed" tokens
-            for tokid in healed_tokens[:-1]:
-              self._logits = self._eval(tokid)
+            self._logits = self._eval_mult(healed_tokens[:-1])
             self._next_token = (healed_tokens[-1], self.decode(healed_tokens[-1:]))
             return len(healed_tokens) - 1
         else:
-          for tokid in healed_tokens:
-            self._logits = self._eval(tokid)
+          self._logits = self._eval_mult(healed_tokens)
           init_offset = 1
-        
-      for tokid in input_ids[init_offset:-1]:
-        self._logits = self._eval(tokid)
-      num_toks += len(input_ids) - init_offset - 1
-      self._next_token = (input_ids[-1], self.decode(input_ids[-1:]))
+      
+      if len(tokens) - init_offset - 1 != 0:
+        self._logits = self._eval_mult(tokens[init_offset:-1])
+        num_toks += len(tokens) - init_offset - 1
+      self._next_token = (tokens[-1], self.decode(tokens[-1:]))
     else:
       if self._next_token is not None:
         tokid, tokstr = self._next_token
         self._eval(tokid)
         num_toks += 1
-      for tokid in input_ids:
-        self._logits = self._eval(tokid)
-      num_toks += len(input_ids)
+      self._logits = self._eval_mult(tokens)
+      num_toks += len(tokens)
 
     return num_toks
 
 T_Embedding = TypeVar('T_Embedding')
 
 class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_Embedding]):
   """ Session for a language model that outputs an embedding for raw text. """
```

### Comparing `langdash-0.0.4.dev2/langdash/models/mock.py` & `langdash-0.0.5.dev1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/models/rwkvcpp.py` & `langdash-0.0.5.dev1/langdash/models/rwkvcpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,51 +138,62 @@
   def _next_token_probs(self) -> torch.Tensor:
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       logits, _ = self._rwkv.eval(self._next_token[0], self._state)
-    return torch.nn.functional.softmax(logits, dim=-1)
+    return sampling.logits_to_probs(logits)
 
-  def _infer(self,
-            end: Optional[Union[str, int]],
-            args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
+  def _infer(
+    self,
+    end: Optional[Union[str, int]],
+    args: InferArgs) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
     stops_at_eot = (
       (isinstance(end, str) and len(end) == 0) or
       (isinstance(end, int) and end == 0)
     )
     
+    if self._logits is None:
+      raise ValueError("no prompt provided for RWKVCppModel")
+    
     for i in range(args.max_new_tokens):
       strip_left = 0
       
       if i == 0 and self._next_token is not None:
-        _, tokstr = self._next_token
-        for key, value in self._tokenizer.get_vocab().items():
-          if not key.startswith(tokstr):
-            self._logits[value] = -inf
-        strip_left = len(tokstr)
-      
+        tokid, tokstr = self._next_token
+        
+        for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
+          if not logits_tokstr.startswith(tokstr):
+            self._logits[logits_tokid] = -inf
+            
+        if self._logits.isinf().all():
+          # we don't need to heal tokens because no token that begins with _next_token
+          self._logits, self._state = self._rwkv.eval(tokid, self._state)
+        else:
+          strip_left = len(tokstr)
+        
       if not stops_at_eot: # no early endoftext
         self._logits[0] = -inf
-        
+      
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
       
       if tokid == end: # implies end is int
         break
       
-      tokstr = self._tokenizer.decode([tokid])
-      
       if stops_at_eot and tokid == 0:
         break
-      elif "\ufffd" in tokstr:
+      
+      tokstr = self._tokenizer.decode([tokid])
+      
+      if "\ufffd" in tokstr:
         buffered_tokens.append(tokid)
         self._next_token = (tokid, "")
       else:
         if buffered_tokens:
           tokstr = self._tokenizer.decode(buffered_tokens)
           tokstr += self._tokenizer.decode([tokid])
           buffered_tokens.clear()
@@ -197,14 +208,16 @@
           generated = generated[:-len(end)]
           break
         
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
         
       self._logits, self._state = self._rwkv.eval(tokid, self._state)
     
+    if buffered_tokens:
+      generated += self._tokenizer.decode(buffered_tokens)
     yield RespInfer(tokid=0, tokstr="", running_infer=generated)
 
 class RWKVCppModel(LLM[RWKVCppSession]):
   """
   rwkv.cpp model
   """
```

### Comparing `langdash-0.0.4.dev2/langdash/models/sentence_transformers.py` & `langdash-0.0.5.dev1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/models/transformers.py` & `langdash-0.0.5.dev1/langdash/models/transformers.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,46 +96,49 @@
       logits = self._logits
     else:
       logits = self._model.forward(
         torch.IntTensor([self._next_token[0]]),
         past_key_values=self._past_key_values,
         use_cache=True
       )._logits[-1]
-    return torch.nn.functional.softmax(logits, dim=-1)
+    return sampling.logits_to_probs(logits)
   
   def _infer(self,
             end: Optional[Union[str, int]],
             args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
     stops_at_eot = (
       (isinstance(end, str) and len(end) == 0) or
       (isinstance(end, int) and end == self._tokenizer.eos_token_id)
     )
     
     for i in range(args.max_new_tokens):
-      postprocess_fn = None
+      strip_left = 0
       
       if i == 0 and self._next_token is not None:
-        _, tokstr = self._next_token
+        tokid, tokstr = self._next_token
+        
         if tokstr == " ":
-          for key, value in self._tokenizer.get_vocab().items():
+          for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
             #https://github.com/openai/gpt-2/issues/80
             #starts with 0x120
-            if key.startswith(self._space_token):
-              self._logits[value] = -inf
-          postprocess_fn = lambda x: " " + x
+            if logits_tokstr.startswith(self._space_token):
+              self._logits[logits_tokid] = -inf
+          strip_left = 1
         else:
-          for key, value in self._tokenizer.get_vocab().items():
-            if not key.startswith(tokstr):
-              self._logits[value] = -inf
-          _tokstr_len = len(tokstr)
-          postprocess_fn = lambda x: x[_tokstr_len:]
-        # self._next_token = None
+          for logits_tokstr, logits_tokid in self._tokenizer.get_vocab().items():
+            if not logits_tokstr.startswith(tokstr):
+              self._logits[logits_tokid] = -inf
+          strip_left = len(tokstr)
+          
+        if self._logits.isinf().all():
+          # we don't need to heal tokens because no token that begins with _next_token
+          self._logits = self._eval(tokid)
       
       if not stops_at_eot: # no early endoftext
         self._logits[0] = -inf
       
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
       
@@ -146,16 +149,16 @@
       else:
         if buffered_tokens:
           tokstr = self._tokenizer.decode(buffered_tokens + [tokid])
           buffered_tokens = []
         else:
           tokstr = self._tokenizer.decode([tokid])
         
-        if postprocess_fn is not None:
-          tokstr = postprocess_fn(tokstr)
+        if strip_left:
+          tokstr = tokstr[strip_left:]
         
         self._next_token = (tokid, tokstr)
         
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
```

### Comparing `langdash-0.0.4.dev2/langdash/response.py` & `langdash-0.0.5.dev1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/sampling.py` & `langdash-0.0.5.dev1/langdash/sampling.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,15 +64,18 @@
 def sample(*args, **kwargs) -> int:
   """
   Sample from a distribution of tokens specified by *logits*.
   
   Args:
     logits (torch.FloatTensor): Logits to sample from.
     args (InferArgs): Sampling arguments.
-    ctx (List[int]): List of current tokens generated.
+    ctx (List[int]): List of tokens generated so far.
   
   Returns:
-    The token generated.
+    The token sampled.
   """
   probs = _output_probs(*args, **kwargs)
   return int(torch.multinomial(probs, num_samples=1)[0])
-  
+  
+def logits_to_probs(logits: torch.Tensor):
+  """ Converts logit tensor to probability tensor using softmax. """
+  return torch.nn.functional.softmax(logits, dim=-1)
```

### Comparing `langdash-0.0.4.dev2/langdash/search/embedding_search.py` & `langdash-0.0.5.dev1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash/search/multichoice_search.py` & `langdash-0.0.5.dev1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.4.dev2/langdash.egg-info/PKG-INFO` & `langdash-0.0.5.dev1/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.4.dev2
+Version: 0.0.5.dev1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: embeddings
 Provides-Extra: rwkvcpp
+Provides-Extra: llamacpp
 Provides-Extra: transformers
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
 A simple library for interfacing with language models.
```

### Comparing `langdash-0.0.4.dev2/langdash.egg-info/SOURCES.txt` & `langdash-0.0.5.dev1/langdash.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 langdash.egg-info/SOURCES.txt
 langdash.egg-info/dependency_links.txt
 langdash.egg-info/requires.txt
 langdash.egg-info/top_level.txt
 langdash/classify/__init__.py
 langdash/classify/token_qa.py
 langdash/models/__init__.py
+langdash/models/llamacpp.py
 langdash/models/mock.py
 langdash/models/rwkvcpp.py
 langdash/models/sentence_transformers.py
 langdash/models/transformers.py
 langdash/search/__init__.py
 langdash/search/embedding_search.py
 langdash/search/engine.py
```

### Comparing `langdash-0.0.4.dev2/setup.py` & `langdash-0.0.5.dev1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,11 +38,12 @@
     ],
     extras_require={
       # Modules
       "embeddings": ["faiss"],
           
       # Backend
       "rwkvcpp": ["tokenizers"],
+      "llamacpp": ["llama-cpp-python==0.1.57"],
       "transformers": ["transformers"],
       "sentence_transformers": ["sentence_transformers"],
     },
 )
```

