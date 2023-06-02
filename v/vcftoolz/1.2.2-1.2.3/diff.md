# Comparing `tmp/vcftoolz-1.2.2.tar.gz` & `tmp/vcftoolz-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcftoolz-1.2.2.tar", last modified: Thu Jun  1 05:38:38 2023, max compression
+gzip compressed data, was "vcftoolz-1.2.3.tar", last modified: Fri Jun  2 03:25:31 2023, max compression
```

## Comparing `vcftoolz-1.2.2.tar` & `vcftoolz-1.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:38.065079 vcftoolz-1.2.2/
--rwxrwxrwx   0 chet      (1000) chet      (1000)      220 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/AUTHORS.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     3327 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/CONTRIBUTING.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     1027 2023-06-01 05:26:46.000000 vcftoolz-1.2.2/HISTORY.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     1556 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/LICENSE
--rwxrwxrwx   0 chet      (1000) chet      (1000)      244 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/MANIFEST.in
--rw-r--r--   0 chet      (1000) chet      (1000)     3984 2023-06-01 05:38:38.067082 vcftoolz-1.2.2/PKG-INFO
--rwxrwxrwx   0 chet      (1000) chet      (1000)     1954 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/README.rst
-drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.520564 vcftoolz-1.2.2/docs/
--rwxrwxrwx   0 chet      (1000) chet      (1000)     6770 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/Makefile
--rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/authors.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     9411 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/conf.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)       33 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/contributing.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/history.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)      451 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/index.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)      713 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/installation.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     6463 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/make.bat
--rwxrwxrwx   0 chet      (1000) chet      (1000)       27 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/readme.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     8624 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/usage.rst
-drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.603562 vcftoolz-1.2.2/pyvenn/
--rw-r--r--   0 chet      (1000) chet      (1000)        0 2023-06-01 04:52:05.000000 vcftoolz-1.2.2/pyvenn/__init__.py
--rw-r--r--   0 chet      (1000) chet      (1000)     1184 2023-06-01 04:52:05.000000 vcftoolz-1.2.2/pyvenn/demo.py
--rw-r--r--   0 chet      (1000) chet      (1000)    22120 2023-06-01 04:52:05.000000 vcftoolz-1.2.2/pyvenn/venn.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)      159 2023-06-01 05:38:38.075079 vcftoolz-1.2.2/setup.cfg
--rwxr-xr-x   0 chet      (1000) chet      (1000)     1887 2023-06-01 05:11:11.000000 vcftoolz-1.2.2/setup.py
-drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.691563 vcftoolz-1.2.2/tests/
--rwxrwxrwx   0 chet      (1000) chet      (1000)       24 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/tests/__init__.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)      299 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/tests/test_cli.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)     3198 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/tests/test_vcftoolz.py
-drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.811081 vcftoolz-1.2.2/vcftoolz/
--rwxrwxrwx   0 chet      (1000) chet      (1000)      113 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/__init__.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)    13994 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/cli.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)    28430 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/vcf_call_parser.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)    45814 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/vcftoolz.py
-drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:38.033082 vcftoolz-1.2.2/vcftoolz.egg-info/
--rw-r--r--   0 chet      (1000) chet      (1000)     3984 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/PKG-INFO
--rw-r--r--   0 chet      (1000) chet      (1000)      674 2023-06-01 05:38:37.000000 vcftoolz-1.2.2/vcftoolz.egg-info/SOURCES.txt
--rw-r--r--   0 chet      (1000) chet      (1000)        1 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/dependency_links.txt
--rw-r--r--   0 chet      (1000) chet      (1000)       48 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/entry_points.txt
--rw-r--r--   0 chet      (1000) chet      (1000)        1 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/not-zip-safe
--rw-r--r--   0 chet      (1000) chet      (1000)       57 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/requires.txt
--rw-r--r--   0 chet      (1000) chet      (1000)       16 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/top_level.txt
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-02 03:25:31.666845 vcftoolz-1.2.3/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      220 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/AUTHORS.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3327 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/CONTRIBUTING.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1104 2023-06-02 03:15:44.000000 vcftoolz-1.2.3/HISTORY.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1556 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/LICENSE
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      244 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/MANIFEST.in
+-rw-r--r--   0 chet      (1000) chet      (1000)     4041 2023-06-02 03:25:31.667846 vcftoolz-1.2.3/PKG-INFO
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1954 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/README.rst
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-02 03:25:31.232398 vcftoolz-1.2.3/docs/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     6770 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/Makefile
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/authors.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     9411 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/conf.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       33 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/contributing.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/history.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      451 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/index.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      713 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/installation.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     6463 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/make.bat
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       27 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/readme.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     8624 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/docs/usage.rst
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-02 03:25:31.307399 vcftoolz-1.2.3/pyvenn/
+-rw-r--r--   0 chet      (1000) chet      (1000)        0 2023-06-01 04:52:05.000000 vcftoolz-1.2.3/pyvenn/__init__.py
+-rw-r--r--   0 chet      (1000) chet      (1000)     1184 2023-06-01 04:52:05.000000 vcftoolz-1.2.3/pyvenn/demo.py
+-rw-r--r--   0 chet      (1000) chet      (1000)    22124 2023-06-02 03:09:37.000000 vcftoolz-1.2.3/pyvenn/venn.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      159 2023-06-02 03:25:31.674616 vcftoolz-1.2.3/setup.cfg
+-rwxr-xr-x   0 chet      (1000) chet      (1000)     1887 2023-06-02 03:15:52.000000 vcftoolz-1.2.3/setup.py
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-02 03:25:31.381846 vcftoolz-1.2.3/tests/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       24 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/tests/__init__.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      299 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/tests/test_cli.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3198 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/tests/test_vcftoolz.py
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-02 03:25:31.475349 vcftoolz-1.2.3/vcftoolz/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      113 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/vcftoolz/__init__.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    13994 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/vcftoolz/cli.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    28404 2023-06-02 03:07:18.000000 vcftoolz-1.2.3/vcftoolz/vcf_call_parser.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    45814 2023-05-05 03:49:57.000000 vcftoolz-1.2.3/vcftoolz/vcftoolz.py
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-02 03:25:31.642354 vcftoolz-1.2.3/vcftoolz.egg-info/
+-rw-r--r--   0 chet      (1000) chet      (1000)     4041 2023-06-02 03:25:30.000000 vcftoolz-1.2.3/vcftoolz.egg-info/PKG-INFO
+-rw-r--r--   0 chet      (1000) chet      (1000)      674 2023-06-02 03:25:30.000000 vcftoolz-1.2.3/vcftoolz.egg-info/SOURCES.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)        1 2023-06-02 03:25:30.000000 vcftoolz-1.2.3/vcftoolz.egg-info/dependency_links.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)       47 2023-06-02 03:25:30.000000 vcftoolz-1.2.3/vcftoolz.egg-info/entry_points.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)        1 2023-06-02 03:25:30.000000 vcftoolz-1.2.3/vcftoolz.egg-info/not-zip-safe
+-rw-r--r--   0 chet      (1000) chet      (1000)       57 2023-06-02 03:25:30.000000 vcftoolz-1.2.3/vcftoolz.egg-info/requires.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)       16 2023-06-02 03:25:30.000000 vcftoolz-1.2.3/vcftoolz.egg-info/top_level.txt
```

### Comparing `vcftoolz-1.2.2/CONTRIBUTING.rst` & `vcftoolz-1.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/HISTORY.rst` & `vcftoolz-1.2.3/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 History
 =======
 
+1.2.3 (2023-06-02)
+------------------
+* Fixed imports in our fork of pyvenn
+
 1.2.2 (2023-06-01)
 ------------------
 * Fixed broken Pyvenn dependency
 
 1.2.1 (2023-05-09)
 ------------------
 * Update PyVCF to PyVCF3
```

### Comparing `vcftoolz-1.2.2/LICENSE` & `vcftoolz-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/PKG-INFO` & `vcftoolz-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vcftoolz
-Version: 1.2.2
+Version: 1.2.3
 Summary: Tools for working with Variant Call Format files.
 Home-page: https://github.com/CFSAN-Biostatistics/vcftoolz
 Author: Steve Davis
 Author-email: steven.davis@fda.hhs.gov
 License: BSD
 Keywords: bioinformatics,NGS,vcftoolz
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -83,14 +82,18 @@
 
 
 
 
 History
 =======
 
+1.2.3 (2023-06-02)
+------------------
+* Fixed imports in our fork of pyvenn
+
 1.2.2 (2023-06-01)
 ------------------
 * Fixed broken Pyvenn dependency
 
 1.2.1 (2023-05-09)
 ------------------
 * Update PyVCF to PyVCF3
@@ -116,9 +119,7 @@
 * Support reading gzip compressed vcf files.
 
 
 1.0.0 (2018-11-20)
 ---------------------
 
 * First public release.
-
-
```

### Comparing `vcftoolz-1.2.2/README.rst` & `vcftoolz-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/docs/Makefile` & `vcftoolz-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/docs/conf.py` & `vcftoolz-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/docs/installation.rst` & `vcftoolz-1.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/docs/make.bat` & `vcftoolz-1.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/docs/usage.rst` & `vcftoolz-1.2.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/pyvenn/demo.py` & `vcftoolz-1.2.3/pyvenn/demo.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/pyvenn/venn.py` & `vcftoolz-1.2.3/pyvenn/venn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 from itertools import chain
-from collections import Iterable
+from collections.abc import Iterable
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 from matplotlib import colors
 import math
 
 default_colors = [
     # r, g, b, a
```

### Comparing `vcftoolz-1.2.2/setup.py` & `vcftoolz-1.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 test_requirements = [
     "pytest",
 ]
 
 setup(
     name='vcftoolz',
-    version='1.2.2',
+    version='1.2.3',
     description="Tools for working with Variant Call Format files.",
     long_description=readme + '\n\n' + history,
     author="Steve Davis",
     author_email='steven.davis@fda.hhs.gov',
     url='https://github.com/CFSAN-Biostatistics/vcftoolz',
     packages=[
         'pyvenn',
```

### Comparing `vcftoolz-1.2.2/tests/test_vcftoolz.py` & `vcftoolz-1.2.3/tests/test_vcftoolz.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/vcftoolz/cli.py` & `vcftoolz-1.2.3/vcftoolz/cli.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/vcftoolz/vcf_call_parser.py` & `vcftoolz-1.2.3/vcftoolz/vcf_call_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -494,57 +494,57 @@
     call : pyvcf call
         Genotype call parsed by PyVCF.
 
     Examples
     --------
     >>> # snp when snps included
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 1/1:PASS", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=1/1, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=1/1, FT=[]))
     >>> # snp when snps excluded
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 1/1:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # indel when snps included
     >>> _test_call_generator("chrom 1 . A AT . PASS . GT:FT 1/1:PASS", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # ref call when snps included
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 0/0:PASS", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # insertion when indels included
     >>> _test_call_generator("chrom 1 . A AT . PASS . GT:FT 1/1:PASS", exclude_snps=True, exclude_indels=False, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=A, ALT=[AT]) Call(sample=SAMPLE, CallData(GT=1/1, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=A, ALT=[AT]) Call(sample=SAMPLE, CallData(GT=1/1, FT=[]))
     >>> # insertion when indels excluded
     >>> _test_call_generator("chrom 1 . A AT . PASS . GT:FT 1/1:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # deletion when indels included
     >>> _test_call_generator("chrom 1 . AT A . PASS . GT:FT 1/1:PASS", exclude_snps=True, exclude_indels=False, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=AT, ALT=[A]) Call(sample=SAMPLE, CallData(GT=1/1, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=AT, ALT=[A]) Call(sample=SAMPLE, CallData(GT=1/1, FT=[]))
     >>> # deletion when indels excluded
     >>> _test_call_generator("chrom 1 . AT A . PASS . GT:FT 1/1:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # structural variant when "other variants" included
     >>> _test_call_generator("chrom 1 . AT A . PASS SVTYPE=DEL; GT:FT 1/1:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=False, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=AT, ALT=[A]) Call(sample=SAMPLE, CallData(GT=1/1, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=AT, ALT=[A]) Call(sample=SAMPLE, CallData(GT=1/1, FT=[]))
     >>> # structural variant when "other variants" excluded
     >>> _test_call_generator("chrom 1 . AT A . PASS SVTYPE=DEL; GT:FT 1/1:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # ref call when ref calls included
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 0/0:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=True, exclude_refs=False, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=0/0, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=0/0, FT=[]))
     >>> # ref call when ref calls excluded
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 0/0:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # heterozygous snp call when snps and heterozygous calls included
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 0/1:PASS", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=False, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=0/1, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=0/1, FT=[]))
     >>> # heterozygous snp call when snps included, but heterozygous calls excluded
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 0/1:PASS", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # FT filtered snp when snps and filtered calls included
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 1/1:FAIL", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=False, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=1/1, FT=FAIL))
+    Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=1/1, FT=['FAIL']))
     >>> # FT filtered snp when snps included, but filtered calls excluded
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:FT 1/1:FAIL", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
 
     >>> # FILTER filtered snp when snps and filtered calls included
     >>> _test_call_generator("chrom 1 . A T . FAIL . GT 1/1", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=False, exclude_missing=True)
     Record(CHROM=chrom, POS=1, REF=A, ALT=[T]) Call(sample=SAMPLE, CallData(GT=1/1))
     >>> # FILTER filtered snp when snps included, but filtered calls excluded
@@ -558,31 +558,31 @@
     >>> # missing call when missing calls excluded
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:DP:FT ./.:.:.", exclude_snps=False, exclude_indels=False, exclude_vars=False, exclude_refs=False, exclude_hetero=False, exclude_filtered=False, exclude_missing=True)
 
     >>> _test_call_generator("chrom 1 . A T . PASS . GT:DP:FT .:.:.", exclude_snps=False, exclude_indels=False, exclude_vars=False, exclude_refs=False, exclude_hetero=False, exclude_filtered=False, exclude_missing=True)
 
     >>> # mix of snps and indels in same record, all calls are homozygous
     >>> _test_call_generator("chrom 1 . T G,TGA . PASS . GT:FT 1/1:PASS 2/2:PASS", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE1, CallData(GT=1/1, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE1, CallData(GT=1/1, FT=[]))
     >>> _test_call_generator("chrom 1 . T G,TGA . PASS . GT:FT 1/1:PASS 2/2:PASS", exclude_snps=True, exclude_indels=False, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE2, CallData(GT=2/2, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE2, CallData(GT=2/2, FT=[]))
     >>> _test_call_generator("chrom 1 . T G,TGA . PASS . GT:FT 1/1:PASS 2/2:PASS", exclude_snps=False, exclude_indels=False, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE1, CallData(GT=1/1, FT=PASS))
-    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE2, CallData(GT=2/2, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE1, CallData(GT=1/1, FT=[]))
+    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE2, CallData(GT=2/2, FT=[]))
     >>> _test_call_generator("chrom 1 . T G,TGA . PASS . GT:FT 2/2:PASS 1/1:PASS", exclude_snps=False, exclude_indels=False, exclude_vars=True, exclude_refs=True, exclude_hetero=True, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE1, CallData(GT=2/2, FT=PASS))
-    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE2, CallData(GT=1/1, FT=PASS))
+    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE1, CallData(GT=2/2, FT=[]))
+    Record(CHROM=chrom, POS=1, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE2, CallData(GT=1/1, FT=[]))
 
     >>> # mix of heterozygous snps and indels in same call
     >>> _test_call_generator("chrom 2 . T G,TGA . PASS . GT:FT 1/2:PASS", exclude_snps=False, exclude_indels=False, exclude_vars=True, exclude_refs=True, exclude_hetero=False, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=2, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE, CallData(GT=1/2, FT=PASS))
+    Record(CHROM=chrom, POS=2, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE, CallData(GT=1/2, FT=[]))
     >>> _test_call_generator("chrom 2 . T G,TGA . PASS . GT:FT 1/2:PASS", exclude_snps=False, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=False, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=2, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE, CallData(GT=1/2, FT=PASS))
+    Record(CHROM=chrom, POS=2, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE, CallData(GT=1/2, FT=[]))
     >>> _test_call_generator("chrom 2 . T G,TGA . PASS . GT:FT 1/2:PASS", exclude_snps=True, exclude_indels=False, exclude_vars=True, exclude_refs=True, exclude_hetero=False, exclude_filtered=True, exclude_missing=True)
-    Record(CHROM=chrom, POS=2, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE, CallData(GT=1/2, FT=PASS))
+    Record(CHROM=chrom, POS=2, REF=T, ALT=[G, TGA]) Call(sample=SAMPLE, CallData(GT=1/2, FT=[]))
     >>> _test_call_generator("chrom 2 . T G,TGA . PASS . GT:FT 1/2:PASS", exclude_snps=True, exclude_indels=True, exclude_vars=True, exclude_refs=True, exclude_hetero=False, exclude_filtered=True, exclude_missing=True)
 
     """
     reader = vcf.VCFReader(input)
     for record in reader:
         for call in record.samples:
             # All calls are included by default, unless explicitly excluded
```

### Comparing `vcftoolz-1.2.2/vcftoolz/vcftoolz.py` & `vcftoolz-1.2.3/vcftoolz/vcftoolz.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.2/vcftoolz.egg-info/PKG-INFO` & `vcftoolz-1.2.3/vcftoolz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vcftoolz
-Version: 1.2.2
+Version: 1.2.3
 Summary: Tools for working with Variant Call Format files.
 Home-page: https://github.com/CFSAN-Biostatistics/vcftoolz
 Author: Steve Davis
 Author-email: steven.davis@fda.hhs.gov
 License: BSD
 Keywords: bioinformatics,NGS,vcftoolz
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Freely Distributable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -83,14 +82,18 @@
 
 
 
 
 History
 =======
 
+1.2.3 (2023-06-02)
+------------------
+* Fixed imports in our fork of pyvenn
+
 1.2.2 (2023-06-01)
 ------------------
 * Fixed broken Pyvenn dependency
 
 1.2.1 (2023-05-09)
 ------------------
 * Update PyVCF to PyVCF3
@@ -116,9 +119,7 @@
 * Support reading gzip compressed vcf files.
 
 
 1.0.0 (2018-11-20)
 ---------------------
 
 * First public release.
-
-
```

### Comparing `vcftoolz-1.2.2/vcftoolz.egg-info/SOURCES.txt` & `vcftoolz-1.2.3/vcftoolz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

