# Comparing `tmp/nanoqa-0.0.37.tar.gz` & `tmp/nanoqa-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoqa-0.0.37.tar", max compression
+gzip compressed data, was "nanoqa-0.0.40.tar", max compression
```

## Comparing `nanoqa-0.0.37.tar` & `nanoqa-0.0.40.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11357 2023-02-27 18:49:46.633525 nanoqa-0.0.37/LICENSE
--rw-r--r--   0        0        0     1337 2023-05-14 13:11:48.178895 nanoqa-0.0.37/README.md
--rw-r--r--   0        0        0      313 2023-05-14 13:11:48.179223 nanoqa-0.0.37/nanoqa/__init__.py
--rw-r--r--   0        0        0        0 2023-02-11 10:39:47.389576 nanoqa-0.0.37/nanoqa/components/__init__.py
--rw-r--r--   0        0        0       48 2023-05-14 13:11:48.180046 nanoqa-0.0.37/nanoqa/components/document_store/__init__.py
--rw-r--r--   0        0        0    15469 2023-05-14 13:11:48.180849 nanoqa-0.0.37/nanoqa/components/document_store/lexical.py
--rw-r--r--   0        0        0      132 2023-05-14 13:11:48.181141 nanoqa-0.0.37/nanoqa/components/file_processing/__init__.py
--rw-r--r--   0        0        0       92 2023-05-14 13:11:48.181258 nanoqa-0.0.37/nanoqa/components/file_processing/convertors/__init__.py
--rw-r--r--   0        0        0      603 2023-05-14 13:11:48.181365 nanoqa-0.0.37/nanoqa/components/file_processing/convertors/docx.py
--rw-r--r--   0        0        0     2002 2023-05-14 13:11:48.182025 nanoqa-0.0.37/nanoqa/components/file_processing/convertors/pdf.py
--rw-r--r--   0        0        0      315 2023-05-14 13:11:48.182242 nanoqa-0.0.37/nanoqa/components/file_processing/convertors/txt.py
--rw-r--r--   0        0        0       39 2023-05-14 13:11:48.188080 nanoqa-0.0.37/nanoqa/components/file_processing/text_processor/__init__.py
--rw-r--r--   0        0        0     6603 2023-05-14 13:11:48.188985 nanoqa-0.0.37/nanoqa/components/file_processing/text_processor/preprocessor.py
--rw-r--r--   0        0        0      395 2023-02-11 10:39:47.521107 nanoqa-0.0.37/nanoqa/components/file_processing/utils.py
--rw-r--r--   0        0        0     2225 2023-05-14 13:11:48.189168 nanoqa-0.0.37/nanoqa/components/file_processing/x2pdf.py
--rw-r--r--   0        0        0      118 2023-05-14 13:11:48.189312 nanoqa-0.0.37/nanoqa/components/question_answering/__init__.py
--rw-r--r--   0        0        0        0 2023-02-11 10:39:47.391279 nanoqa-0.0.37/nanoqa/components/question_answering/handlers/__init__.py
--rw-r--r--   0        0        0     8661 2023-05-14 13:11:48.189484 nanoqa-0.0.37/nanoqa/components/question_answering/handlers/inference.py
--rw-r--r--   0        0        0     6136 2023-05-14 13:11:48.189630 nanoqa-0.0.37/nanoqa/components/question_answering/handlers/train.py
--rw-r--r--   0        0        0       50 2023-05-14 13:11:48.194993 nanoqa-0.0.37/nanoqa/components/question_answering/pipeline/__init__.py
--rw-r--r--   0        0        0    14646 2023-05-14 13:11:48.195600 nanoqa-0.0.37/nanoqa/components/question_answering/pipeline/es.py
--rw-r--r--   0        0        0       34 2023-05-14 13:11:48.195732 nanoqa-0.0.37/nanoqa/components/question_answering/ranker/__init__.py
--rw-r--r--   0        0        0     1859 2023-05-14 13:11:48.196378 nanoqa-0.0.37/nanoqa/components/question_answering/ranker/cross_encoder.py
--rw-r--r--   0        0        0       49 2023-02-27 18:49:46.637196 nanoqa-0.0.37/nanoqa/components/question_answering/reader/__init__.py
--rw-r--r--   0        0        0     4023 2023-05-14 13:11:48.196512 nanoqa-0.0.37/nanoqa/components/question_answering/reader/adapter.py
--rw-r--r--   0        0        0     3970 2023-05-14 13:13:23.317531 nanoqa-0.0.37/nanoqa/components/question_answering/reader/base.py
--rw-r--r--   0        0        0       28 2023-05-14 13:11:48.197221 nanoqa-0.0.37/nanoqa/components/question_answering/retriever/__init__.py
--rw-r--r--   0        0        0     1907 2023-05-14 13:11:48.197338 nanoqa-0.0.37/nanoqa/components/question_answering/retriever/base.py
--rw-r--r--   0        0        0     1012 2023-05-14 13:11:48.197457 nanoqa-0.0.37/nanoqa/components/question_answering/tokenization.py
--rw-r--r--   0        0        0     3360 2023-05-14 13:11:48.197582 nanoqa-0.0.37/nanoqa/components/rich_utils.py
--rw-r--r--   0        0        0       82 2023-02-27 18:49:46.638059 nanoqa-0.0.37/nanoqa/configs.py
--rw-r--r--   0        0        0      239 2023-05-14 13:11:48.197687 nanoqa-0.0.37/nanoqa/schemas/__init__.py
--rw-r--r--   0        0        0       63 2023-05-14 13:11:48.197792 nanoqa-0.0.37/nanoqa/schemas/pipeline/__init__.py
--rw-r--r--   0        0        0      639 2023-02-11 10:39:47.564676 nanoqa-0.0.37/nanoqa/schemas/pipeline/pipeline_schemas.py
--rw-r--r--   0        0        0      148 2023-05-14 13:11:48.197898 nanoqa-0.0.37/nanoqa/schemas/reader/__init__.py
--rw-r--r--   0        0        0      554 2023-02-11 10:39:47.507198 nanoqa-0.0.37/nanoqa/schemas/reader/reader_args.py
--rw-r--r--   0        0        0     2383 2023-05-14 13:11:48.198002 nanoqa-0.0.37/nanoqa/schemas/reader/reader_schemas.py
--rw-r--r--   0        0        0       51 2023-05-14 13:11:48.198098 nanoqa-0.0.37/nanoqa/schemas/retriever/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-14 13:11:48.198288 nanoqa-0.0.37/nanoqa/schemas/retriever/retriever_schemas.py
--rw-r--r--   0        0        0   168260 2023-02-27 18:49:46.640064 nanoqa-0.0.37/nanoqa/static/Roboto-Regular.ttf
--rw-r--r--   0        0        0     1013 2023-05-14 13:12:20.197576 nanoqa-0.0.37/pyproject.toml
--rw-r--r--   0        0        0     2947 1970-01-01 00:00:00.000000 nanoqa-0.0.37/setup.py
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 nanoqa-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 18:49:46.633525 nanoqa-0.0.40/LICENSE
+-rw-r--r--   0        0        0     1337 2023-05-14 13:11:48.178895 nanoqa-0.0.40/README.md
+-rw-r--r--   0        0        0      313 2023-05-14 13:11:48.179223 nanoqa-0.0.40/nanoqa/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-11 10:39:47.389576 nanoqa-0.0.40/nanoqa/components/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-14 13:11:48.180046 nanoqa-0.0.40/nanoqa/components/document_store/__init__.py
+-rw-r--r--   0        0        0    15469 2023-05-14 13:11:48.180849 nanoqa-0.0.40/nanoqa/components/document_store/lexical.py
+-rw-r--r--   0        0        0      132 2023-05-14 13:11:48.181141 nanoqa-0.0.40/nanoqa/components/file_processing/__init__.py
+-rw-r--r--   0        0        0       92 2023-05-14 13:11:48.181258 nanoqa-0.0.40/nanoqa/components/file_processing/convertors/__init__.py
+-rw-r--r--   0        0        0      603 2023-05-14 13:11:48.181365 nanoqa-0.0.40/nanoqa/components/file_processing/convertors/docx.py
+-rw-r--r--   0        0        0     2002 2023-05-14 13:11:48.182025 nanoqa-0.0.40/nanoqa/components/file_processing/convertors/pdf.py
+-rw-r--r--   0        0        0      315 2023-05-14 13:11:48.182242 nanoqa-0.0.40/nanoqa/components/file_processing/convertors/txt.py
+-rw-r--r--   0        0        0       39 2023-05-14 13:11:48.188080 nanoqa-0.0.40/nanoqa/components/file_processing/text_processor/__init__.py
+-rw-r--r--   0        0        0     6603 2023-05-14 13:11:48.188985 nanoqa-0.0.40/nanoqa/components/file_processing/text_processor/preprocessor.py
+-rw-r--r--   0        0        0      395 2023-02-11 10:39:47.521107 nanoqa-0.0.40/nanoqa/components/file_processing/utils.py
+-rw-r--r--   0        0        0     2225 2023-05-14 13:11:48.189168 nanoqa-0.0.40/nanoqa/components/file_processing/x2pdf.py
+-rw-r--r--   0        0        0      118 2023-05-14 13:31:11.123772 nanoqa-0.0.40/nanoqa/components/question_answering/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-11 10:39:47.391279 nanoqa-0.0.40/nanoqa/components/question_answering/handlers/__init__.py
+-rw-r--r--   0        0        0     8661 2023-05-14 13:11:48.189484 nanoqa-0.0.40/nanoqa/components/question_answering/handlers/inference.py
+-rw-r--r--   0        0        0     6136 2023-05-14 13:11:48.189630 nanoqa-0.0.40/nanoqa/components/question_answering/handlers/train.py
+-rw-r--r--   0        0        0       50 2023-05-14 13:11:48.194993 nanoqa-0.0.40/nanoqa/components/question_answering/pipeline/__init__.py
+-rw-r--r--   0        0        0    14601 2023-05-14 14:01:58.944239 nanoqa-0.0.40/nanoqa/components/question_answering/pipeline/es.py
+-rw-r--r--   0        0        0       34 2023-05-14 13:11:48.195732 nanoqa-0.0.40/nanoqa/components/question_answering/ranker/__init__.py
+-rw-r--r--   0        0        0     2000 2023-06-02 19:01:07.858909 nanoqa-0.0.40/nanoqa/components/question_answering/ranker/cross_encoder.py
+-rw-r--r--   0        0        0       49 2023-02-27 18:49:46.637196 nanoqa-0.0.40/nanoqa/components/question_answering/reader/__init__.py
+-rw-r--r--   0        0        0     4101 2023-06-02 18:59:45.471483 nanoqa-0.0.40/nanoqa/components/question_answering/reader/adapter.py
+-rw-r--r--   0        0        0     4133 2023-06-02 18:59:33.365201 nanoqa-0.0.40/nanoqa/components/question_answering/reader/base.py
+-rw-r--r--   0        0        0       28 2023-05-14 13:11:48.197221 nanoqa-0.0.40/nanoqa/components/question_answering/retriever/__init__.py
+-rw-r--r--   0        0        0     1907 2023-05-14 13:11:48.197338 nanoqa-0.0.40/nanoqa/components/question_answering/retriever/base.py
+-rw-r--r--   0        0        0     1012 2023-05-14 13:11:48.197457 nanoqa-0.0.40/nanoqa/components/question_answering/tokenization.py
+-rw-r--r--   0        0        0     3360 2023-05-14 13:11:48.197582 nanoqa-0.0.40/nanoqa/components/rich_utils.py
+-rw-r--r--   0        0        0       82 2023-02-27 18:49:46.638059 nanoqa-0.0.40/nanoqa/configs.py
+-rw-r--r--   0        0        0      239 2023-05-14 13:11:48.197687 nanoqa-0.0.40/nanoqa/schemas/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-14 13:11:48.197792 nanoqa-0.0.40/nanoqa/schemas/pipeline/__init__.py
+-rw-r--r--   0        0        0      639 2023-02-11 10:39:47.564676 nanoqa-0.0.40/nanoqa/schemas/pipeline/pipeline_schemas.py
+-rw-r--r--   0        0        0      148 2023-05-14 13:11:48.197898 nanoqa-0.0.40/nanoqa/schemas/reader/__init__.py
+-rw-r--r--   0        0        0      554 2023-02-11 10:39:47.507198 nanoqa-0.0.40/nanoqa/schemas/reader/reader_args.py
+-rw-r--r--   0        0        0     2383 2023-05-14 13:11:48.198002 nanoqa-0.0.40/nanoqa/schemas/reader/reader_schemas.py
+-rw-r--r--   0        0        0       51 2023-05-14 13:11:48.198098 nanoqa-0.0.40/nanoqa/schemas/retriever/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-14 13:11:48.198288 nanoqa-0.0.40/nanoqa/schemas/retriever/retriever_schemas.py
+-rw-r--r--   0        0        0   168260 2023-02-27 18:49:46.640064 nanoqa-0.0.40/nanoqa/static/Roboto-Regular.ttf
+-rw-r--r--   0        0        0      785 2023-06-02 19:02:00.733790 nanoqa-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0     2947 1970-01-01 00:00:00.000000 nanoqa-0.0.40/setup.py
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 nanoqa-0.0.40/PKG-INFO
```

### Comparing `nanoqa-0.0.37/LICENSE` & `nanoqa-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/README.md` & `nanoqa-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/document_store/lexical.py` & `nanoqa-0.0.40/nanoqa/components/document_store/lexical.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/file_processing/convertors/docx.py` & `nanoqa-0.0.40/nanoqa/components/file_processing/convertors/docx.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/file_processing/convertors/pdf.py` & `nanoqa-0.0.40/nanoqa/components/file_processing/convertors/pdf.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/file_processing/text_processor/preprocessor.py` & `nanoqa-0.0.40/nanoqa/components/file_processing/text_processor/preprocessor.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/file_processing/x2pdf.py` & `nanoqa-0.0.40/nanoqa/components/file_processing/x2pdf.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/handlers/inference.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/handlers/inference.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/handlers/train.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/handlers/train.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/pipeline/es.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/pipeline/es.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 import re
 import time
 import unicodedata
 from typing import Dict, List, Optional
 
 import torch.cuda
 
-from ....schemas import (
-    Document,
-    FinalPrediction,
-    PipelineAnswer,
-    PipelineResponse,
-    ReaderArguments,
-)
 from ...document_store import ElasticsearchDocumentStore as DocumentStore
 from ...question_answering import Ranker, Reader, Retriever
 from ...rich_utils import (
     display_answers,
     display_json,
     display_retrieved_documents,
     display_time_taken,
 )
+from ....schemas import (
+    Document,
+    FinalPrediction,
+    PipelineAnswer,
+    PipelineResponse,
+    ReaderArguments,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class ElasticSearchPipeline:
     def __init__(
         self,
         model_name_or_path: str,
         index_name: str,
-        username: str,
-        password: str,
         index_hash: str,
         reader_args: ReaderArguments,
-        ca_certs: str = Optional[str],
-        http_auth: str = Optional[str],
+        ca_certs: str = None,
+        http_auth: str = None,
+        username: str = None,
+        password: str = None,
         verify_certs: bool = True,
         use_ranker: bool = True,
         top_k_ranker: int = 50,
         use_gpu: bool = True,
         es_host: str = "localhost",
         es_port: int = 9200,
         skip_detailed_features: bool = True,
@@ -75,24 +75,23 @@
         self.reader = self._init_reader()
         self.ranker = self._init_ranker()
 
         self.display_pipeline_params()
         self.pad_token = self.reader.tokenizer.pad_token
 
     def _init_document_store(self) -> DocumentStore:
-        index = self.index_name or self.index_hash
         return DocumentStore(
             username=self.username,
             password=self.password,
             ca_certs=self.ca_certs,
             http_auth=self.http_auth,
             verify_certs=self.verify_certs,
             host=self.es_host,
             port=self.es_port,
-            index=index,
+            index=self.index_hash,
         )
 
     def display_pipeline_params(self):
         # display attributes of Pipeline class, if they are among string, int, float, bool
         display_json(
             data={
                 k: v
```

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/ranker/cross_encoder.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/ranker/cross_encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from typing import List
+from typing import List, Union
 
 import torch
 from transformers import AutoModelForSequenceClassification, AutoTokenizer
 
 from ....schemas import Document
 
 
 class Ranker:
     def __init__(
         self,
         model_name_or_path: str = "cross-encoder/mmarco-mMiniLMv2-L12-H384-v1",
         max_seq_len: int = 384,
         use_gpu: bool = False,
+        use_auth_token: Union[str, bool] = False,
     ):
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
+        self.tokenizer = AutoTokenizer.from_pretrained(
+            model_name_or_path, use_auth_token=use_auth_token
+        )
         self.model = AutoModelForSequenceClassification.from_pretrained(
-            model_name_or_path
+            model_name_or_path, use_auth_token=use_auth_token
         )
         self.max_seq_len = max_seq_len
         self.device = (
             torch.device("cuda")
             if use_gpu and torch.cuda.is_available()
             else torch.device("cpu")
         )
```

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/reader/adapter.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/reader/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         use_gpu: bool = True,
         nbest_from_chunk: int = 3,
         nbest_from_document: int = 1,
         return_no_answer: bool = False,
         no_ans_boost: float = 0.0,
         skip_detailed_features: bool = True,
         display_progress_bar: bool = True,
+        use_auth_token: Union[str, bool] = False,
     ):
         """
         :param model_name_or_path: name of the model to load or path to a directory containing model files
         :param max_seq_len: maximum length of the sequence to be considered by the model
         :param doc_stride: stride to be used while splitting the document into chunks
         :param max_ans_len: maximum length of the answer to be considered by the model
         :param use_gpu: whether to use GPU or not
@@ -45,14 +46,15 @@
             use_gpu,
             nbest_from_chunk,
             nbest_from_document,
             return_no_answer,
             no_ans_boost,
             skip_detailed_features,
             display_progress_bar,
+            use_auth_token,
         )
 
     def load_adapter(self, adapter_location: Union[str, Path]):
         if isinstance(adapter_location, Path):
             adapter_location = str(adapter_location)
         adapter_name = self.model.load_adapter(adapter_location, with_head=False)
         self.model.qa_outputs.load_state_dict(
```

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/reader/base.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/reader/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import replace
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import torch
 from transformers import AutoModelForQuestionAnswering, AutoTokenizer, BatchEncoding
 
 from ....schemas import FinalPrediction, ReaderArguments
 from ..handlers.inference import model_inference, multi_documents_aggregation
 from ..tokenization import tokenization_question_contexts
@@ -19,21 +19,26 @@
         use_gpu: bool = True,
         nbest_from_chunk: int = 3,
         nbest_from_document: int = 1,
         return_no_answer: bool = False,
         no_ans_boost: float = 0.0,
         skip_detailed_features: bool = True,
         display_progress_bar: bool = True,
+        use_auth_token: Union[str, bool] = False,
     ):
         self.use_gpu = use_gpu
         self.device = torch.device(
             "cuda" if torch.cuda.is_available() and use_gpu else "cpu"
         )
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
-        self.model = AutoModelForQuestionAnswering.from_pretrained(model_name_or_path)
+        self.tokenizer = AutoTokenizer.from_pretrained(
+            model_name_or_path, use_auth_token=use_auth_token
+        )
+        self.model = AutoModelForQuestionAnswering.from_pretrained(
+            model_name_or_path, use_auth_token=use_auth_token
+        )
         self.reader_args = ReaderArguments(
             max_seq_len=max_seq_len,
             doc_stride=doc_stride,
             max_ans_len=max_ans_len,
             nbest_from_chunk=nbest_from_chunk,
             nbest_from_document=nbest_from_document,
             return_no_answer=return_no_answer,
```

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/retriever/base.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/retriever/base.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/question_answering/tokenization.py` & `nanoqa-0.0.40/nanoqa/components/question_answering/tokenization.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/components/rich_utils.py` & `nanoqa-0.0.40/nanoqa/components/rich_utils.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/schemas/pipeline/pipeline_schemas.py` & `nanoqa-0.0.40/nanoqa/schemas/pipeline/pipeline_schemas.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/schemas/reader/reader_args.py` & `nanoqa-0.0.40/nanoqa/schemas/reader/reader_args.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/schemas/reader/reader_schemas.py` & `nanoqa-0.0.40/nanoqa/schemas/reader/reader_schemas.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/schemas/retriever/retriever_schemas.py` & `nanoqa-0.0.40/nanoqa/schemas/retriever/retriever_schemas.py`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/nanoqa/static/Roboto-Regular.ttf` & `nanoqa-0.0.40/nanoqa/static/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nanoqa-0.0.37/setup.py` & `nanoqa-0.0.40/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'wheel==0.38.4']
 
 entry_points = \
 {'console_scripts': ['cli_command_name = package_name:function']}
 
 setup_kwargs = {
     'name': 'nanoqa',
-    'version': '0.0.37',
+    'version': '0.0.40',
     'description': '',
     'long_description': '<div align="center"> \n    <h1>\n        Question Answering kit\n    </h1>\n</div>\n\n## Requirements\n\n    - python >= 3.8\n\n```bash\n# python environment\nwhich python3\npython3 -m venv nanoEnv\nsource ./nanoEnv/bin/activate\n\n# m1 chip, problem shooting pyserini installation\n# CFLAGS="-mavx -DWARN(a)=(a)" pip install nmslib \n\n# pip3 upgrade\npip3 install --upgrade pip\npip3 install -r requirements.txt\n\n# we also need to install tessaract library, well google it for your os\n## For Linux\nsudo apt install tesseract-ocr -y\nsudo apt install tesseract-ocr-heb\nsudo apt install tesseract-ocr-all -y\n```\n\n    - Elasticsearch\n\n```bash\n# run elasticsearch in a docker container\ndocker run -d -p 127.0.0.1:9200:9200 -p 127.0.0.1:9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.9.2\n# after creation of the container, run the following command to start the container\ndocker start <container_id>\n```\n\n## Todos\n\n- [X] Migrate/Re-Implement full QA functions\n- [X] Implementation of pdf conversion.\n- [X] Implementation of file extraction.\n- [X] Implementation of Retriever via ElasticSearch\n- [X] Implementation of fine-tuning the reader with adapter\n- [X] Put tests\n\n# Download WikiDump\n\n```bash\npython download_wikidump.py --lang en --latest --delete-dump \n```\n\n\n## ChangeLog\n\n- 2023-03-02: replace xpdf by PyMuPDF\n',
     'author': 'Kunpeng GUO',
     'author_email': 'gabin.guo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/gabinguo/nanoQA',
```

### Comparing `nanoqa-0.0.37/PKG-INFO` & `nanoqa-0.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoqa
-Version: 0.0.37
+Version: 0.0.40
 Summary: 
 Home-page: https://github.com/gabinguo/nanoQA
 License: Apache
 Keywords: Question Answering,Huggingface Transformers
 Author: Kunpeng GUO
 Author-email: gabin.guo@gmail.com
 Requires-Python: >=3.8,<4.0
```

