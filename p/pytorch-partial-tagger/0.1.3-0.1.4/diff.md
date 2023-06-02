# Comparing `tmp/pytorch_partial_tagger-0.1.3.tar.gz` & `tmp/pytorch_partial_tagger-0.1.4.tar.gz`

## Comparing `pytorch_partial_tagger-0.1.3.tar` & `pytorch_partial_tagger-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/notebooks/basic.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/__about__.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/embedders.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/matchers.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/recognizer.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/tagger.py
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/training.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/utils.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/__init__.py
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/functional.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/nn.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/data/__init__.py
--rw-r--r--   0        0        0     8725 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/data/batch.py
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/data/core.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/decoders/__init__.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/decoders/viterbi.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/__init__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/base.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/linear.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/crf/__init__.py
--rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/crf/test_functional.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/crf/test_nn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/data/__init__.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/data/test_batch.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/tests/data/test_core.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/LICENSE
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/README.md
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/notebooks/basic.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/__about__.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/embedders.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/matchers.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/recognizer.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/tagger.py
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/training.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/utils.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/__init__.py
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/functional.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/nn.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/data/__init__.py
+-rw-r--r--   0        0        0     8725 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/data/batch.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/data/core.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/decoders/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/decoders/viterbi.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/__init__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/base.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/linear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/crf/__init__.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/crf/test_functional.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/crf/test_nn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/data/__init__.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/data/test_batch.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/tests/data/test_core.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/README.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 pytorch_partial_tagger-0.1.4/PKG-INFO
```

### Comparing `pytorch_partial_tagger-0.1.3/.github/workflows/ci.yml` & `pytorch_partial_tagger-0.1.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/.github/workflows/pypi-publish.yml` & `pytorch_partial_tagger-0.1.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/notebooks/basic.ipynb` & `pytorch_partial_tagger-0.1.4/notebooks/basic.ipynb`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/embedders.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/embedders.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/matchers.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/matchers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/recognizer.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/recognizer.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/tagger.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/tagger.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/training.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/training.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/utils.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/functional.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/crf/nn.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/crf/nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/data/batch.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/data/batch.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/data/core.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/data/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,14 +152,20 @@
                 self.get_tag_size(),
                 self.__status_kind,
             )
         ]
 
         self.__label_ids = dict(zip(self.__labels, self.__start_indices))
 
+    def __contains__(self, label: str) -> bool:
+        i = bisect_left(self.__labels, label)
+        if i >= len(self.__labels):
+            return False
+        return self.__labels[i] == label
+
     def get_outside_index(self) -> int:
         return 0
 
     def get_start_index(self, label: str) -> int:
         if label not in self.__label_ids:
             raise ValueError("Invalid label is given.")
         return self.__label_ids[label]
@@ -169,14 +175,17 @@
 
     def get_end_index(self, label: str) -> int:
         return self.get_start_index(label) + 2
 
     def get_unit_index(self, label: str) -> int:
         return self.get_start_index(label) + 3
 
+    def get_labels(self) -> list:
+        return self.__labels
+
     def get_label_size(self) -> int:
         return len(self.__labels)
 
     def get_tag_size(self) -> int:
         # (start, inside, end, unit) * label + outside status
         return self.__status_kind * self.get_label_size() + 1
```

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/decoders/viterbi.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/decoders/viterbi.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/base.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/base.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/src/partial_tagger/encoders/linear.py` & `pytorch_partial_tagger-0.1.4/src/partial_tagger/encoders/linear.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/tests/conftest.py` & `pytorch_partial_tagger-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/tests/helpers.py` & `pytorch_partial_tagger-0.1.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/tests/crf/test_functional.py` & `pytorch_partial_tagger-0.1.4/tests/crf/test_functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/tests/crf/test_nn.py` & `pytorch_partial_tagger-0.1.4/tests/crf/test_nn.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/tests/data/test_batch.py` & `pytorch_partial_tagger-0.1.4/tests/data/test_batch.py`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/tests/data/test_core.py` & `pytorch_partial_tagger-0.1.4/tests/data/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,32 @@
 
 
 @pytest.fixture
 def label_set() -> LabelSet:
     return LabelSet({"ORG", "PER"})
 
 
+@pytest.mark.parametrize(
+    "label, expected",
+    [
+        ("ORG", True),
+        ("PER", True),
+        ("PERSON", False),
+        ("LOCATION", False),
+        ("ORGANIZE", False),
+    ],
+)
+def test_membership_check_is_valid(
+    label_set: LabelSet, label: str, expected: bool
+) -> None:
+    is_member = label in label_set
+
+    assert is_member == expected
+
+
 def test_tokens_are_valid(tokenized_text: TokenizedText) -> None:
     token_indices = [1, 2, 3, 4, 5, 6, 7, 8]
     expected = ["Tok", "yo", "is", "the", "capital", "of", "Japan", "."]
 
     tokens = []
     for token_index in token_indices:
         tokens.append(tokenized_text.get_token(token_index))
```

### Comparing `pytorch_partial_tagger-0.1.3/.gitignore` & `pytorch_partial_tagger-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/LICENSE` & `pytorch_partial_tagger-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/README.md` & `pytorch_partial_tagger-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_partial_tagger-0.1.3/pyproject.toml` & `pytorch_partial_tagger-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,14 @@
   "F",  # pyflakes
   "I",  # isort
   "C",  # flake8-comprehensions
   "B",  # flake8-bugbear
 ]
 src = ["src"]
 
-[tool.ruff.isort]
-known-third-party = ["partial-tagger"]
-
 [tool.ruff.mccabe]
 max-complexity = 18
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 show_error_codes = true
```

### Comparing `pytorch_partial_tagger-0.1.3/PKG-INFO` & `pytorch_partial_tagger-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-partial-tagger
-Version: 0.1.3
+Version: 0.1.4
 Summary: Sequence Tagger for Partially Annotated Dataset in PyTorch
 Project-URL: Homepage, https://github.com/yasufumy/pytorch-partial-tagger
 Author-email: Yasufumi Taniguchi <yasufumi.taniguchi@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

