# Comparing `tmp/pytorch_partial_tagger-0.1.4.tar.gz` & `tmp/pytorch_partial_tagger-0.1.5.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.4.tar` & `pytorch_partial_tagger-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/notebooks/basic.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/embedders.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/training.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/utils.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0     8725 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/data/batch.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/linear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/crf/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/crf/test_functional.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/crf/test_nn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/data/__init__.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/data/test_batch.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/data/test_core.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/LICENSE
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/README.md
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/notebooks/basic.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/embedders.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/__init__.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/core.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/tag.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/data/batch/text.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/linear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/data/__init__.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/data/test_batch.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/tests/data/test_core.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/README.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.5/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.4/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.1.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/notebooks/basic.ipynb` & `pytorch_partial_tagger-0.1.5/notebooks/basic.ipynb`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/embedders.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/embedders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABCMeta, abstractmethod
 
 import torch
 from torch import nn
 from transformers import PreTrainedModel
 
-from .data.batch import TaggerInputs
+from .data.batch.text import TaggerInputs
 
 
 class BaseEmbedder(nn.Module, metaclass=ABCMeta):
     """Base class of all embedders."""
 
     @abstractmethod
     def forward(self, inputs: TaggerInputs) -> torch.Tensor:
```

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/recognizer.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/recognizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import cast
 
 import torch
 from torch.utils.data import DataLoader
 
-from .data.batch import BaseBatchFactory, Batch, CharBasedTagsCollection, Texts
+from .data.batch import Batch, BatchFactory
+from .data.batch.tag import CharBasedTagsCollection
+from .data.batch.text import Texts
 from .tagger import SequenceTagger
 
 
 class Recognizer:
     def __init__(
         self,
         tagger: SequenceTagger,
-        batch_factory: BaseBatchFactory,
+        batch_factory: BatchFactory,
         padding_index: int,
     ):
         self.__tagger = tagger
         self.__batch_factory = batch_factory
         self.__padding_index = padding_index
 
     def __call__(
```

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import torch
 from torch.nn import Module
 
 from .crf.nn import CRF
-from .data.batch import TaggerInputs
+from .data.batch.text import TaggerInputs
 from .decoders import ViterbiDecoder
 from .embedders import BaseEmbedder
 from .encoders import BaseEncoder
 
 
 class SequenceTagger(Module):
     """Sequence tagger.
```

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from typing import cast
 
 import torch
 from torch.utils.data import DataLoader
 
 from .crf import functional as F
 from .data import LabelSet
-from .data.batch import Batch, CharBasedTagsCollection, Dataset
+from .data.batch import Batch, Dataset
+from .data.batch.tag import CharBasedTagsCollection
 from .recognizer import Recognizer
 from .utils import Metric, create_collator, create_tagger
 
 
 class SlantedTriangular:
     def __init__(self, max_steps: int, cut_frac: float = 0.1, ratio: int = 16):
         self.__cut_frac = cut_frac
```

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/utils.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from transformers import AutoModel, AutoTokenizer
 
 from .data import LabelSet, Span, Tag
-from .data.batch import CharBasedTagsCollection, Collator, TransformerBatchFactory
+from .data.batch import BatchFactory, Collator
+from .data.batch.tag import CharBasedTagsCollection
+from .data.batch.text import TransformerTokenizer
 from .decoders.viterbi import Contrainer, ViterbiDecoder
 from .embedders import TransformerEmbedder
 from .encoders.linear import LinearEncoder
 from .tagger import SequenceTagger
 
 
 def create_tag(start: int, length: int, label: str) -> Tag:
@@ -59,16 +61,17 @@
     """Creates a collator.
 
     Args:
         model_name: A string representing a transformer's model name.
         label_set: A LabelSet object.
         tokenizer_args: A dictionary representing arguments passed to tokenizer.
     """
-    batch_factory = TransformerBatchFactory(
-        AutoTokenizer.from_pretrained(model_name), label_set, tokenizer_args
+    batch_factory = BatchFactory(
+        TransformerTokenizer(AutoTokenizer.from_pretrained(model_name), tokenizer_args),
+        label_set,
     )
     return Collator(batch_factory)
 
 
 class Metric:
     def __init__(self) -> None:
         self.__tp = 0
```

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/crf/nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/data/core.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/data/core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/decoders/viterbi.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/base.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/linear.py` & `pytorch_partial_tagger-0.1.5/src/partial_tagger/encoders/linear.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/tests/conftest.py` & `pytorch_partial_tagger-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/tests/helpers.py` & `pytorch_partial_tagger-0.1.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.1.5/tests/crf/test_functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.1.5/tests/crf/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/tests/data/test_batch.py` & `pytorch_partial_tagger-0.1.5/tests/data/test_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import pytest
 import torch
 from transformers import AutoTokenizer
 
 from partial_tagger.data import CharBasedTags, LabelSet, Span, Tag
-from partial_tagger.data.batch import TransformerBatchFactory
+from partial_tagger.data.batch import BatchFactory
+from partial_tagger.data.batch.text import TransformerTokenizer
 
 
 @pytest.fixture
-def batch_factory() -> TransformerBatchFactory:
-    return TransformerBatchFactory(
-        AutoTokenizer.from_pretrained("distilroberta-base"),
+def batch_factory() -> BatchFactory:
+    return BatchFactory(
+        TransformerTokenizer(AutoTokenizer.from_pretrained("distilroberta-base")),
         LabelSet({"LOC", "MISC", "ORG", "PER"}),
     )
 
 
-def test_char_based_tags_are_valid(batch_factory: TransformerBatchFactory) -> None:
+def test_char_based_tags_are_valid(batch_factory: BatchFactory) -> None:
     text = "Tokyo is the capital of Japan."
     tag_indices = torch.tensor([[0, 1, 3, 0, 0, 0, 0, 4, 0, 0]])
 
     expected = CharBasedTags(
         (Tag(Span(0, 5), "LOC"), Tag(Span(24, 5), "LOC")), text=text
     )
 
     batch = batch_factory.create((text,))
     char_based_tags_collection = batch.create_char_based_tags(tag_indices)
 
     assert len(char_based_tags_collection) == 1
     assert char_based_tags_collection[0] == expected
 
 
-def test_tag_indices_are_valid(batch_factory: TransformerBatchFactory) -> None:
+def test_tag_indices_are_valid(batch_factory: BatchFactory) -> None:
     text = "Tokyo is the capital of Japan."
     tags = CharBasedTags((Tag(Span(0, 5), "LOC"), Tag(Span(24, 5), "LOC")), text=text)
     unknown_index = -100
 
     expected = torch.tensor([[0, 1, 3, -100, -100, -100, -100, 4, -100, 0]])
 
     batch = batch_factory.create((text,))
```

### Comparing `pytorch_partial_tagger-0.1.4/tests/data/test_core.py` & `pytorch_partial_tagger-0.1.5/tests/data/test_core.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/.gitignore` & `pytorch_partial_tagger-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/LICENSE` & `pytorch_partial_tagger-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/README.md` & `pytorch_partial_tagger-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/pyproject.toml` & `pytorch_partial_tagger-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.4/PKG-INFO` & `pytorch_partial_tagger-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.4
+Version: 0.1.5
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

