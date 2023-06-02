# Comparing `tmp/paper-qa-2.0.2.tar.gz` & `tmp/paper-qa-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-2.0.2.tar", last modified: Wed May 31 21:22:30 2023, max compression
+gzip compressed data, was "paper-qa-2.0.3.tar", last modified: Fri Jun  2 20:24:12 2023, max compression
```

## Comparing `paper-qa-2.0.2.tar` & `paper-qa-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 21:21:47.000000 paper-qa-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-31 21:22:30.689701 paper-qa-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-05-31 21:21:47.000000 paper-qa-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:22:30.689701 paper-qa-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-31 21:21:47.000000 paper-qa-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-05-31 21:21:47.000000 paper-qa-2.0.2/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 20:23:34.000000 paper-qa-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-02 20:24:12.469730 paper-qa-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-06-02 20:23:34.000000 paper-qa-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.465730 paper-qa-2.0.3/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22806 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 20:24:12.469730 paper-qa-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-02 20:23:34.000000 paper-qa-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-06-02 20:23:34.000000 paper-qa-2.0.3/tests/test_paperqa.py
```

### Comparing `paper-qa-2.0.2/LICENSE` & `paper-qa-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/PKG-INFO` & `paper-qa-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.0.2
+Version: 2.0.3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.0.2/README.md` & `paper-qa-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/paper_qa.egg-info/PKG-INFO` & `paper-qa-2.0.3/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.0.2
+Version: 2.0.3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.0.2/paperqa/agent.py` & `paper-qa-2.0.3/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/paperqa/contrib/zotero.py` & `paper-qa-2.0.3/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/paperqa/docs.py` & `paper-qa-2.0.3/paperqa/docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -360,31 +360,42 @@
         max_sources: int = 5,
         marginal_relevance: bool = True,
         key_filter: Optional[List[str]] = None,
         get_callbacks: Callable[[str], AsyncCallbackHandler] = lambda x: [],
     ) -> Answer:
         if len(self.docs) == 0:
             return answer
+        if key_filter is not None:
+            answer.key_filter = key_filter
         if self._faiss_index is None:
             self._build_faiss_index()
         _k = k
-        if key_filter is not None:
+        if answer.key_filter is not None:
             _k = k * 10  # heuristic
         # want to work through indices but less k
         if marginal_relevance:
             docs = self._faiss_index.max_marginal_relevance_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
         else:
             docs = self._faiss_index.similarity_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
         # ok now filter
-        if key_filter is not None:
-            docs = [doc for doc in docs if doc.metadata["dockey"] in key_filter][:k]
+        if answer.key_filter is not None:
+            # I realize that by testing for existence
+            # in strings that weird cases can
+            # happen - like FooBar can match FooBar2023
+            # but remember there are later checks
+            # The risk of explicitly parsing is that the
+            # language model may not give back in predictable
+            # format (e.g., - "FooBar and BarSoo are good papers")
+            docs = [doc for doc in docs if doc.metadata["dockey"] in answer.key_filter][
+                :k
+            ]
 
         async def process(doc):
             if doc.metadata["dockey"] in self._deleted_keys:
                 return None, None
             # check if it is already in answer (possible in agent setting)
             if doc.metadata["key"] in [c.key for c in answer.contexts]:
                 return None, None
@@ -520,20 +531,20 @@
         if len(answer.contexts) == 0:
             if key_filter or (key_filter is None and len(self.docs) > max_sources):
                 callbacks = [OpenAICallbackHandler()] + get_callbacks("filter")
                 keys = await self.adoc_match(answer.question, callbacks=callbacks)
                 answer.tokens += callbacks[0].total_tokens
                 answer.cost += callbacks[0].total_cost
                 key_filter = True if len(keys) > 0 else False
+                answer.key_filter = keys
             answer = await self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
-                key_filter=keys if key_filter else None,
                 get_callbacks=get_callbacks,
             )
         context_str, contexts = answer.context, answer.contexts
         bib = dict()
         passages = dict()
         if len(context_str) < 10:
             answer_text = (
```

### Comparing `paper-qa-2.0.2/paperqa/qaprompts.py` & `paper-qa-2.0.3/paperqa/qaprompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/paperqa/readers.py` & `paper-qa-2.0.3/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/paperqa/types.py` & `paper-qa-2.0.3/paperqa/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Union, Optional
 
 StrPath = Union[str, Path]
 
 
 @dataclass
 class Context:
     """A class to hold the context of a question."""
@@ -29,14 +29,15 @@
     context: str = ""
     contexts: List[Context] = None
     references: str = ""
     formatted_answer: str = ""
     passages: Dict[str, str] = None
     tokens: int = 0
     cost: float = 0
+    key_filter: Optional[str] = None
 
     def __post_init__(self):
         """Initialize the answer."""
         if self.contexts is None:
             self.contexts = []
         if self.passages is None:
             self.passages = {}
```

### Comparing `paper-qa-2.0.2/paperqa/utils.py` & `paper-qa-2.0.3/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/setup.py` & `paper-qa-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.2/tests/test_paperqa.py` & `paper-qa-2.0.3/tests/test_paperqa.py`

 * *Files identical despite different names*

