# Comparing `tmp/streq-0.0.1.tar.gz` & `tmp/streq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streq-0.0.1.tar", last modified: Tue May 16 10:47:20 2023, max compression
+gzip compressed data, was "streq-0.0.2.tar", last modified: Fri Jun  2 11:14:41 2023, max compression
```

## Comparing `streq-0.0.1.tar` & `streq-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:47:20.918447 streq-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 10:47:09.000000 streq-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 10:47:20.918447 streq-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-16 10:47:09.000000 streq-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 10:47:09.000000 streq-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:47:20.918447 streq-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:47:20.918447 streq-0.0.1/streq/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 10:47:09.000000 streq-0.0.1/streq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-16 10:47:09.000000 streq-0.0.1/streq/circular.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-16 10:47:09.000000 streq-0.0.1/streq/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-16 10:47:09.000000 streq-0.0.1/streq/seqtools.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-16 10:47:09.000000 streq-0.0.1/streq/sequences.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-16 10:47:09.000000 streq-0.0.1/streq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:47:20.918447 streq-0.0.1/streq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 10:47:20.000000 streq-0.0.1/streq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 10:47:20.000000 streq-0.0.1/streq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:47:20.000000 streq-0.0.1/streq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 10:47:20.000000 streq-0.0.1/streq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 10:47:20.000000 streq-0.0.1/streq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:47:20.918447 streq-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-16 10:47:09.000000 streq-0.0.1/test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:41.377365 streq-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-02 11:14:29.000000 streq-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-02 11:14:41.377365 streq-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 11:14:29.000000 streq-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-02 11:14:29.000000 streq-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:14:41.377365 streq-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:41.377365 streq-0.0.2/streq/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 11:14:29.000000 streq-0.0.2/streq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-02 11:14:29.000000 streq-0.0.2/streq/circular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-02 11:14:29.000000 streq-0.0.2/streq/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-02 11:14:29.000000 streq-0.0.2/streq/seqtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-02 11:14:29.000000 streq-0.0.2/streq/sequences.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-02 11:14:29.000000 streq-0.0.2/streq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:41.377365 streq-0.0.2/streq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-02 11:14:41.000000 streq-0.0.2/streq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 11:14:41.000000 streq-0.0.2/streq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:14:41.000000 streq-0.0.2/streq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 11:14:41.000000 streq-0.0.2/streq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 11:14:41.000000 streq-0.0.2/streq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:41.377365 streq-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-02 11:14:29.000000 streq-0.0.2/test/tests.py
```

### Comparing `streq-0.0.1/LICENSE` & `streq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streq-0.0.1/PKG-INFO` & `streq-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic utilities for working with nucleotide sequence strings.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,158 +27,175 @@
 Project-URL: Homepage, https://github.com/scbirlab/streq
 Project-URL: Bug Tracker, https://github.com/scbirlab/streq/issues
 Keywords: nucleotide,sequence,science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🧬 streq
 
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/scbirlab/streq/python-publish.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/streq)
+![PyPI](https://img.shields.io/pypi/v/streq)
+
 Python utilities for working with nucleotide sequence strings.
 
 ## Installation
 
 ### The easy way
 
 Install the pre-compiled version from PyPI:
 
-```
+```bash
 pip install streq
 ```
 
 ### From source
 
 Clone the repository, then `cd` into it. Then run:
 
-```
+```bash
 pip install -e .
 ```
 
 ## Usage
 
 Streq provides various utility functions in Python for working with nucleotide sequences. 
 Sequences can be upper or lower case, and case will be preserved through transformations.
 
 ### Transformations
 
 Reverse complement.
 
-```
+```python
 >>> import streq as sq
 >>>
 >>> sq.reverse_complement('ATCG')
 'CGAT'
 ```
 
 Convert between RNA and DNA alphabets.
 
-```
+```python
 >>> sq.to_rna('ATCG')
 'AUCG'
 >>> sq.to_dna('AUCG')
 'ATCG'
 ```
 
 Slice circular sequences such as plasmids or bacterial genomes.
 
-```
+```python
 >>> sq.Circular('ATCG')[-1:3]
 'GATC'
 >>> sq.reverse_complement(sq.Circular('ATCG'))[-1:3]
 'CGAT'
 ```
 
 Cases are preserved throughout the transformations.
 
-```
+```python
 >>> sq.reverse_complement(sq.Circular('ATCg'))
 'cGAT'
 ```
 
 ### Calculations
 
 Get GC and pyrimidine content.
 
-```
+```python
 >>> sq.gc_content('AGGG')
 0.75
 >>> sq.pyrimidine_content('AUGGG')
 0.2
 ```
 
 Get autocorrelation (rough indicator for secondary structure).
 
-```
+```python
 >>> sq.correlation('AACC')
 0.0
 >>> sq.correlation('AAATTT')
 2.3
 >>> sq.correlation('AAATTCT')
 1.3047619047619046
 >>> sq.correlation('AAACTTT')
 1.9238095238095236
 ```
 
-Provide a second sequence to get correlation between sequences.
+Wobble base-pairing can be taken into account.
 
+```python
+>>> correlation('GGGTTT')
+0.0
+>>> correlation('GGGTTT', wobble=True)
+2.3
+>>> correlation('GGGUUU', wobble=True)
+2.3
 ```
+
+Provide a second sequence to get correlation between sequences.
+
+```python
 >>> sq.correlation('AAA', 'TTT')
 0.0
 >>> sq.correlation('AAA', 'AAA')
 3.0
 ```
 
 ### Distances
 
 Calculate Levenshtein (insert, delete, mutate) distance.
 
-```
+```python
 >>> sq.levenshtein('AAATTT', 'AAATTT')
 0
 >>> sq.levenshtein('AAATTT', 'ACTTT')
 2
 >>> sq.levenshtein('AAAG', 'TCGA')
 4
 ```
 
 Calculate Hamming (mismatch) distance.
 
-```
+```python
 >>> sq.hamming('AAA', 'ATA')
 1
 >>> sq.hamming('AAA', 'ATT')
 2
 >>> sq.hamming('AAA', 'TTT')
 3
 ```
 
 ### Search
 
 Search sequences using IUPAC symbols and iterate through the results.
 
-```
+```python
 >>> for (start, end), match in sq.find_iupac('ARY', 'AATAGCAGTGTGAAC'):
 ...     print(f"Found ARY at {start}:{end}: {match}")
 ... 
 Found ARY at 0:3: AAT
 Found ARY at 3:6: AGC
 Found ARY at 6:9: AGT
 Found ARY at 12:15: AAC
 ```
 
 Find common Type IIS restriction sites:
 
-```
+```python
 >>> sq.which_re_sites('AAAGAAG')
 ()
 >>> sq.which_re_sites('AAAGAAGAC')
 ('BbsI',)
 >>> sq.which_re_sites('AAAGAAGACACCTGC')
 ('BbsI', 'PaqCI')
 ```
```

### Comparing `streq-0.0.1/README.md` & `streq-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,159 @@
 # 🧬 streq
 
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/scbirlab/streq/python-publish.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/streq)
+![PyPI](https://img.shields.io/pypi/v/streq)
+
 Python utilities for working with nucleotide sequence strings.
 
 ## Installation
 
 ### The easy way
 
 Install the pre-compiled version from PyPI:
 
-```
+```bash
 pip install streq
 ```
 
 ### From source
 
 Clone the repository, then `cd` into it. Then run:
 
-```
+```bash
 pip install -e .
 ```
 
 ## Usage
 
 Streq provides various utility functions in Python for working with nucleotide sequences. 
 Sequences can be upper or lower case, and case will be preserved through transformations.
 
 ### Transformations
 
 Reverse complement.
 
-```
+```python
 >>> import streq as sq
 >>>
 >>> sq.reverse_complement('ATCG')
 'CGAT'
 ```
 
 Convert between RNA and DNA alphabets.
 
-```
+```python
 >>> sq.to_rna('ATCG')
 'AUCG'
 >>> sq.to_dna('AUCG')
 'ATCG'
 ```
 
 Slice circular sequences such as plasmids or bacterial genomes.
 
-```
+```python
 >>> sq.Circular('ATCG')[-1:3]
 'GATC'
 >>> sq.reverse_complement(sq.Circular('ATCG'))[-1:3]
 'CGAT'
 ```
 
 Cases are preserved throughout the transformations.
 
-```
+```python
 >>> sq.reverse_complement(sq.Circular('ATCg'))
 'cGAT'
 ```
 
 ### Calculations
 
 Get GC and pyrimidine content.
 
-```
+```python
 >>> sq.gc_content('AGGG')
 0.75
 >>> sq.pyrimidine_content('AUGGG')
 0.2
 ```
 
 Get autocorrelation (rough indicator for secondary structure).
 
-```
+```python
 >>> sq.correlation('AACC')
 0.0
 >>> sq.correlation('AAATTT')
 2.3
 >>> sq.correlation('AAATTCT')
 1.3047619047619046
 >>> sq.correlation('AAACTTT')
 1.9238095238095236
 ```
 
-Provide a second sequence to get correlation between sequences.
+Wobble base-pairing can be taken into account.
 
+```python
+>>> correlation('GGGTTT')
+0.0
+>>> correlation('GGGTTT', wobble=True)
+2.3
+>>> correlation('GGGUUU', wobble=True)
+2.3
 ```
+
+Provide a second sequence to get correlation between sequences.
+
+```python
 >>> sq.correlation('AAA', 'TTT')
 0.0
 >>> sq.correlation('AAA', 'AAA')
 3.0
 ```
 
 ### Distances
 
 Calculate Levenshtein (insert, delete, mutate) distance.
 
-```
+```python
 >>> sq.levenshtein('AAATTT', 'AAATTT')
 0
 >>> sq.levenshtein('AAATTT', 'ACTTT')
 2
 >>> sq.levenshtein('AAAG', 'TCGA')
 4
 ```
 
 Calculate Hamming (mismatch) distance.
 
-```
+```python
 >>> sq.hamming('AAA', 'ATA')
 1
 >>> sq.hamming('AAA', 'ATT')
 2
 >>> sq.hamming('AAA', 'TTT')
 3
 ```
 
 ### Search
 
 Search sequences using IUPAC symbols and iterate through the results.
 
-```
+```python
 >>> for (start, end), match in sq.find_iupac('ARY', 'AATAGCAGTGTGAAC'):
 ...     print(f"Found ARY at {start}:{end}: {match}")
 ... 
 Found ARY at 0:3: AAT
 Found ARY at 3:6: AGC
 Found ARY at 6:9: AGT
 Found ARY at 12:15: AAC
 ```
 
 Find common Type IIS restriction sites:
 
-```
+```python
 >>> sq.which_re_sites('AAAGAAG')
 ()
 >>> sq.which_re_sites('AAAGAAGAC')
 ('BbsI',)
 >>> sq.which_re_sites('AAAGAAGACACCTGC')
 ('BbsI', 'PaqCI')
 ```
```

### Comparing `streq-0.0.1/pyproject.toml` & `streq-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [project]
 name = "streq"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Eachan Johnson", email="eachan.johnson@crick.ac.uk" },
 ]
 description = "Basic utilities for working with nucleotide sequence strings."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["nucleotide", "sequence", "science"]
 
 classifiers = [  
   
   "Development Status :: 3 - Alpha",
 
   # Indicate who your project is intended for
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Bio-Informatics",
 
   "License :: OSI Approved :: MIT License",
 
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [ 
   "pyyaml"
```

### Comparing `streq-0.0.1/streq/circular.py` & `streq-0.0.2/streq/circular.py`

 * *Files identical despite different names*

### Comparing `streq-0.0.1/streq/distance.py` & `streq-0.0.2/streq/distance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,14 @@
+"""Functions for calculating distances and similarities between sequences."""
+
+from __future__ import annotations
+
+from collections.abc import Callable
 from difflib import SequenceMatcher
+from functools import partial
 
 from .seqtools import reverse_complement
 from .utils import _normalize_case
 
 @_normalize_case(nargs=2)
 def levenshtein(x: str, y: str) -> int:
 
@@ -65,32 +71,28 @@
 							  matrix[i - 1][j - 1])
 				matrix[i][j] = minimum + 1
 
 	return matrix[x_len][y_len]
 
 
 @_normalize_case(nargs=2)
-def hamming(x: str, y: str, 
-	        wobble: bool = False) -> int:
+def hamming(x: str, y: str) -> int:
     
     """Calculate the Hamming distance between two sequences.
     
-    The Hamming distance is the number of mismatches.
-
-    Note: the `wobble` parameter is not yet implemented.
+    The Hamming distance is the number of mismatches for two sequences 
+    of identical length. This function truncates the longer sequence
+    to the shortest length.
 
     Parameters
     ----------
     x : str
         Sequence.
     y : str, optional
         Second sequence for correlation with x.
-    wobble : bool, optional
-        Whether to calulate correlations taking into account G.U wobble.
-        Not yet implemented.
 
     Returns
     -------
     int
         Hamming distance.
 
     Examples
@@ -99,15 +101,15 @@
     1
     >>> hamming('AAA', 'ATT')
     2
     >>> hamming('AAA', 'TTT')
     3
 
     """
-
+    
     return sum(a != b for a, b in zip(x, y))
 
 
 @_normalize_case(nargs=2)
 def ratcliff_obershelp(x: str, 
 					   y: str) -> int:
     
@@ -143,37 +145,52 @@
     """
     
 	sm = SequenceMatcher(a=x, b=y, 
                          autojunk=False).get_opcodes()
     
 	return sum(code[0] != 'equal' for code in sm)
 
+def mismatch_fun(x, y, n, wobble):
+    
+    wobbles = sum(wobble and ((a == 'G' and b == 'A') or (a in 'TU' and b == 'C')) for a, b in zip(x[n:], y))
+    return hamming(x[n:], y) - wobbles
+
+
+def _mismatch_fun(wobble: bool = False) -> Callable[[str, str, int], int]:
+
+    return  partial(mismatch_fun, wobble=wobble)
+
 
 @_normalize_case(nargs=2)
 def correlation(x: str, 
                 y: str = '',
                 wobble: bool = False) -> float:
     
-    """Get autocorrelation of a single sequence or 
+    """Calculate autocorrelation of a single sequence or 
     correlation between two sequences.
 
-    If a single sequence is provided, it's autocorrelation 
-    is calculated, which might be an indicator of secondary structure.
+    If a single sequence is provided, its correlation with its
+    reverse complement is calculated, which might be an indicator 
+    of secondary structure.
+
+    If two sequences are provided, then the correlation between the 
+    first sequence and the reverse complement of the second sequence
+    is calculated. This might be an indicator of binding affinity. 
 
-    Note: the `wobble` parameter is not yet implemented.
+    If wobble is True, then the G.U basepairing is also taken into 
+    account.
 
     Parameters
     ----------
     x : str
         Sequence.
     y : str, optional
         Second sequence for correlation with x.
     wobble : bool, optional
         Whether to calulate correlations taking into account G.U wobble.
-        Not yet implemented.
 
     Returns
     -------
     float
         Correlation.
 
     Examples
@@ -183,20 +200,34 @@
     >>> correlation('AAATTT')
     2.3
     >>> correlation('AAATTCT')
     1.3047619047619046
     >>> correlation('AAACTTT')
     1.9238095238095236
     >>> correlation('AAA', 'TTT')
-    0.0
+    3.0
     >>> correlation('AAA', 'AAA')
+    0.0
+    >>> correlation('GGGTTT')
+    0.0
+    >>> correlation('GGGTTT', wobble=True)
+    2.3
+    >>> correlation('GGGUUU', wobble=True)
+    2.3
+    >>> correlation('GGG', 'UUU')
+    0.0
+    >>> correlation('GGG', 'UUU', wobble=True)
     3.0
 
     """
     
     x = x
-    y = y or reverse_complement(x)
+    y = reverse_complement(y or x)
 
-    max_len = min(len(x), len(y))
-    
-    return sum(((max_len - n) - hamming(x[n:], y, wobble)) / (max_len - n)
-               for n in range(len(x)))
+    len_x = len(x)
+
+    max_len = min(len_x, len(y))
+
+    mismatch_fun = _mismatch_fun(wobble=wobble)
+	    
+    return sum(((max_len - n) - mismatch_fun(x, y, n)) / (max_len - n)
+                for n in range(len_x))
```

### Comparing `streq-0.0.1/streq/seqtools.py` & `streq-0.0.2/streq/seqtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Python utilities for working with nucleotide sequence strings.
 
 Variety of utilities for converting, searching, and doing 
 calculations on nucleotide sequences.
 
 """
 
+from __future__ import annotations
+
 from collections.abc import Generator, Sequence
-from difflib import SequenceMatcher
 import re
 
 from .utils import (sequences, 
                     _preserve_case, 
                     _preserve_circular,
                     _normalize_case)
```

### Comparing `streq-0.0.1/streq/utils.py` & `streq-0.0.2/streq/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Miscellaneous utilities used in streq."""
 
+from __future__ import annotations
+
 from collections import namedtuple
 from collections.abc import Callable, Sequence
 from functools import wraps
 import os
 
 import yaml
```

### Comparing `streq-0.0.1/streq.egg-info/PKG-INFO` & `streq-0.0.2/streq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic utilities for working with nucleotide sequence strings.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,158 +27,175 @@
 Project-URL: Homepage, https://github.com/scbirlab/streq
 Project-URL: Bug Tracker, https://github.com/scbirlab/streq/issues
 Keywords: nucleotide,sequence,science
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🧬 streq
 
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/scbirlab/streq/python-publish.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/streq)
+![PyPI](https://img.shields.io/pypi/v/streq)
+
 Python utilities for working with nucleotide sequence strings.
 
 ## Installation
 
 ### The easy way
 
 Install the pre-compiled version from PyPI:
 
-```
+```bash
 pip install streq
 ```
 
 ### From source
 
 Clone the repository, then `cd` into it. Then run:
 
-```
+```bash
 pip install -e .
 ```
 
 ## Usage
 
 Streq provides various utility functions in Python for working with nucleotide sequences. 
 Sequences can be upper or lower case, and case will be preserved through transformations.
 
 ### Transformations
 
 Reverse complement.
 
-```
+```python
 >>> import streq as sq
 >>>
 >>> sq.reverse_complement('ATCG')
 'CGAT'
 ```
 
 Convert between RNA and DNA alphabets.
 
-```
+```python
 >>> sq.to_rna('ATCG')
 'AUCG'
 >>> sq.to_dna('AUCG')
 'ATCG'
 ```
 
 Slice circular sequences such as plasmids or bacterial genomes.
 
-```
+```python
 >>> sq.Circular('ATCG')[-1:3]
 'GATC'
 >>> sq.reverse_complement(sq.Circular('ATCG'))[-1:3]
 'CGAT'
 ```
 
 Cases are preserved throughout the transformations.
 
-```
+```python
 >>> sq.reverse_complement(sq.Circular('ATCg'))
 'cGAT'
 ```
 
 ### Calculations
 
 Get GC and pyrimidine content.
 
-```
+```python
 >>> sq.gc_content('AGGG')
 0.75
 >>> sq.pyrimidine_content('AUGGG')
 0.2
 ```
 
 Get autocorrelation (rough indicator for secondary structure).
 
-```
+```python
 >>> sq.correlation('AACC')
 0.0
 >>> sq.correlation('AAATTT')
 2.3
 >>> sq.correlation('AAATTCT')
 1.3047619047619046
 >>> sq.correlation('AAACTTT')
 1.9238095238095236
 ```
 
-Provide a second sequence to get correlation between sequences.
+Wobble base-pairing can be taken into account.
 
+```python
+>>> correlation('GGGTTT')
+0.0
+>>> correlation('GGGTTT', wobble=True)
+2.3
+>>> correlation('GGGUUU', wobble=True)
+2.3
 ```
+
+Provide a second sequence to get correlation between sequences.
+
+```python
 >>> sq.correlation('AAA', 'TTT')
 0.0
 >>> sq.correlation('AAA', 'AAA')
 3.0
 ```
 
 ### Distances
 
 Calculate Levenshtein (insert, delete, mutate) distance.
 
-```
+```python
 >>> sq.levenshtein('AAATTT', 'AAATTT')
 0
 >>> sq.levenshtein('AAATTT', 'ACTTT')
 2
 >>> sq.levenshtein('AAAG', 'TCGA')
 4
 ```
 
 Calculate Hamming (mismatch) distance.
 
-```
+```python
 >>> sq.hamming('AAA', 'ATA')
 1
 >>> sq.hamming('AAA', 'ATT')
 2
 >>> sq.hamming('AAA', 'TTT')
 3
 ```
 
 ### Search
 
 Search sequences using IUPAC symbols and iterate through the results.
 
-```
+```python
 >>> for (start, end), match in sq.find_iupac('ARY', 'AATAGCAGTGTGAAC'):
 ...     print(f"Found ARY at {start}:{end}: {match}")
 ... 
 Found ARY at 0:3: AAT
 Found ARY at 3:6: AGC
 Found ARY at 6:9: AGT
 Found ARY at 12:15: AAC
 ```
 
 Find common Type IIS restriction sites:
 
-```
+```python
 >>> sq.which_re_sites('AAAGAAG')
 ()
 >>> sq.which_re_sites('AAAGAAGAC')
 ('BbsI',)
 >>> sq.which_re_sites('AAAGAAGACACCTGC')
 ('BbsI', 'PaqCI')
 ```
```

