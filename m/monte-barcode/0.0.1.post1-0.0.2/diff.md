# Comparing `tmp/monte-barcode-0.0.1.post1.tar.gz` & `tmp/monte-barcode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monte-barcode-0.0.1.post1.tar", last modified: Wed May 17 21:45:06 2023, max compression
+gzip compressed data, was "monte-barcode-0.0.2.tar", last modified: Fri Jun  2 14:26:36 2023, max compression
```

## Comparing `monte-barcode-0.0.1.post1.tar` & `monte-barcode-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/monte_barcode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 21:45:06.000000 monte-barcode-0.0.1.post1/monte_barcode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/montebarcode/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/codons.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/montebarcode/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:45:06.274330 monte-barcode-0.0.1.post1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 21:44:55.000000 monte-barcode-0.0.1.post1/test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:36.090261 monte-barcode-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-06-02 14:26:36.090261 monte-barcode-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16224 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:36.090261 monte-barcode-0.0.2/monte_barcode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-06-02 14:26:36.000000 monte-barcode-0.0.2/monte_barcode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-02 14:26:36.000000 monte-barcode-0.0.2/monte_barcode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:26:36.000000 monte-barcode-0.0.2/monte_barcode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 14:26:36.000000 monte-barcode-0.0.2/monte_barcode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 14:26:36.000000 monte-barcode-0.0.2/monte_barcode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 14:26:36.000000 monte-barcode-0.0.2/monte_barcode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:36.090261 monte-barcode-0.0.2/montebarcode/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/montebarcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/montebarcode/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/montebarcode/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/montebarcode/codons.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/montebarcode/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/montebarcode/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:26:36.090261 monte-barcode-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:36.090261 monte-barcode-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-02 14:26:26.000000 monte-barcode-0.0.2/test/tests.py
```

### Comparing `monte-barcode-0.0.1.post1/LICENSE` & `monte-barcode-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monte-barcode-0.0.1.post1/PKG-INFO` & `monte-barcode-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monte-barcode
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,23 +27,26 @@
 Project-URL: Homepage, https://github.com/scbirlab/monte-barcode
 Project-URL: Bug Tracker, https://github.com/scbirlab/monte-barcode/issues
 Keywords: barcodes,sequencing,science,assay
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
 
 # 🔴🟢🔵⚫️ monte barcode
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/scbirlab/monte-barcode/python-publish.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monte-barcode)
 ![PyPI](https://img.shields.io/pypi/v/monte-barcode)
 
 Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 
 ## Installation
 
@@ -68,15 +71,15 @@
 **monte barcode** provides command line utilities to generate completely random or 
 peptide-encoding barcodes conforming to custom contraints, like minimum edit
 distance among the set, GC content, and color balance for Illumina chemistry.
 
 Barcode sets and individual barcodes are deterministically given an adjective-noun mnemonic 
 (generated by [nemony](https://github.com/scbirlab/nemony)) for easy reference.
 
-Each utility gives a lot of commentary to `stderr`, but the barcodes go to
+Each utility writes a lot of commentary to `stderr`, but the barcodes go to
 `stdout` by default so they can be piped.
 
 ### Command line
 
 Generate random barcodes of a particular length.
 
 ```bash
@@ -169,14 +172,35 @@
 bright_cliff:l6-n10-d3:x6:oceanic_plume AGACTG
 bright_cliff:l6-n10-d3:x7:wanted_jessica        TCTCGA
 bright_cliff:l6-n10-d3:x8:incise_radical        TCTGTC
 bright_cliff:l6-n10-d3:x9:rebel_option  TAGGAC
 Wrote barcode set called bright_cliff, with minimum Hamming distance 3 and maximum Hamming distance 6.
 ```
 
+You can bias sampling based on a set of other sequences. This sampling conditions the choice of each base
+on the previous base.
+
+```bash
+$ monte barcode -n 5 --amino-acid HELP | monte sample --field 2 --distance 2 -n 5
+Generating barcodes with the following parameters:
+        ...
+Requested barcodes with length 12, and 16777216 possible combinations.
+> Tried 12 barcodes, rejected 7, accepted 5; rejection rate is 0.58
+
+Rejection reasons:
+        distance: 0.58
+        gc_content: 0.08
+ritzy_parker:l12-n5-d2:x0:good_race     CACGAATTGCCA
+ritzy_parker:l12-n5-d2:x1:wiry_cairo    CATGAACTACCA
+ritzy_parker:l12-n5-d2:x2:pricy_scuba   CACGAACTGCCT
+ritzy_parker:l12-n5-d2:x3:brisk_neptune CATGAATTGCCG
+ritzy_parker:l12-n5-d2:x4:dextrous_frame        CACGAATTACCG
+Wrote barcode set called ritzy_parker, with minimum Hamming distance 2 and maximum Hamming distance 3.
+```
+
 You can also check and filter previously generated sets.
 
 ```bash
 $ monte barcode --length 6 -n 10 -d 3 2> /dev/null | monte check --color --field 2
 Checking barcodes with the following parameters:
         ...
 > Tried 10 barcodes, rejected 6, accepted 4; rejection rate is 0.60
@@ -187,16 +211,46 @@
 thorough_adam:l6-n4-d4:x1:elfin_rufus   AGCTTC
 thorough_adam:l6-n4-d4:x2:damaged_atlas AAGGCA
 thorough_adam:l6-n4-d4:x3:faded_elite   GCACTA
 Wrote barcode set called thorough_adam, with minimum Hamming distance 4 and maximum Hamming distance 5.
 
 ```
 
-And try to sort by ideal color balance for Illumina chemistries (if you want to use subsets).
+Or use a previous set as a starting point for generating more, possibly with different parameters.
 
+```bash
+$ monte barcode -n10 --distance 4 --length 10  --append <(monte barcode -n 5 -a HELP) --append_field 2
+Generating barcodes with the following parameters:
+...
+> Tried 32 barcodes, rejected 22, accepted 10; rejection rate is 0.69
+
+Rejection reasons:
+        gc_content: 0.44
+        homopolymer: 0.47
+        distance: 0.03
+        palindrome: 0.03
+elegant_triton:l12-n15-d1:x0:vocal_stand        CACGAACTTCCT
+elegant_triton:l12-n15-d1:x1:real_clinic        CATGAATTGCCT
+elegant_triton:l12-n15-d1:x2:dextrous_frame     CACGAATTACCG
+elegant_triton:l12-n15-d1:x3:dizzy_record       CACGAATTACCT
+elegant_triton:l12-n15-d1:x4:prudent_jester     CACGAGCTACCA
+elegant_triton:l10-n15-d1:x5:useful_cabinet     ACGCGACACT
+elegant_triton:l10-n15-d1:x6:deafening_sphere   TAATACGCGC
+elegant_triton:l10-n15-d1:x7:old_program        ATCCTAAGCC
+elegant_triton:l10-n15-d1:x8:eager_doctor       TTGGCCACTG
+elegant_triton:l10-n15-d1:x9:dopey_limbo        ATCCGTCGTA
+elegant_triton:l10-n15-d1:x10:plain_lunar       ACGAGAATTC
+elegant_triton:l10-n15-d1:x11:discreet_ford     CTAACGTAGC
+elegant_triton:l10-n15-d1:x12:proud_jet CTTCAGTGTC
+elegant_triton:l10-n15-d1:x13:wry_insect        CAGACTGGAG
+elegant_triton:l10-n15-d1:x14:lofty_shave       TTCGTAACTC
+Wrote barcode set called elegant_triton, with minimum Hamming distance 1 and maximum Hamming distance 10.
+```
+
+And try to sort by ideal color balance for Illumina chemistries (if you want to use subsets).
 
 ```bash
 $ monte barcode --length 6 -n 15 -d 1 2> /dev/null | monte sort --field 2
 Sorting barcodes with the following parameters:
         ...
 round_mono:l6-n15-d2:x0:shady_soda      AGTCCT
 round_mono:l6-n15-d2:x1:vogue_cosmos    TGAGTC
@@ -215,39 +269,90 @@
 round_mono:l6-n15-d2:x14:discreet_shake GCATTG
 Wrote barcode set called round_mono, with minimum Hamming distance 2 and maximum Hamming distance 6.
 ```
 
 #### Details
 
 ```bash
-usage: monte barcode [-h] --number NUMBER [--length LENGTH] [--rejection-rate REJECTION_RATE]
-                     [--amino-acid AMINO_ACID] [--distance DISTANCE] [--homopolymer HOMOPOLYMER]
-                     [--levenshtein] [--color] [--gc_min GC_MIN] [--gc_max GC_MAX]
-                     [--output OUTPUT]
+usage: monte [-h] {barcode,check,sort,sample} ...
 
-options:
+Generate random DNA barcodes conforming to contraints, or check sets of barcodes for their conformance.
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+Sub-commands:
+  {barcode,check,sort,sample}
+                        Use these commands to specify the action you want.
+    barcode             Generate random barcodes.
+    check               Check barcode list.
+    sort                Sort barcode list for optimal color balance.
+    sample              Generate barcode list by sampling nucleotides from an existing list of sequences.
+```
+
+```bash
+usage: monte barcode [-h] [--length LENGTH] [--amino-acid AMINO_ACID] --number NUMBER [--rejection-rate REJECTION_RATE] [--append APPEND] [--append_field APPEND_FIELD] [--distance DISTANCE]
+                     [--homopolymer HOMOPOLYMER] [--levenshtein] [--color] [--gc_min GC_MIN] [--gc_max GC_MAX] [--output OUTPUT]
+
+optional arguments:
   -h, --help            show this help message and exit
-  --number NUMBER, -n NUMBER
-                        Number of barcodes to generate. Required.
   --length LENGTH, -l LENGTH
                         Barcode length. Default: 12
-  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
-                        Rate of rejection before aborting. Default: 0.85
   --amino-acid AMINO_ACID, -a AMINO_ACID
                         Generate barcodes encoding this amino acid sequence. Default: do not use.
+  --number NUMBER, -n NUMBER
+                        Number of barcodes to generate. Required.
+  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
+                        Rate of rejection before aborting. Default: 0.85
+  --append APPEND       File to take a list of barcodes to extend. Default: do not use
+  --append_field APPEND_FIELD
+                        Column name or number to take barcodes from for appending. Default: 1
+  --distance DISTANCE, -d DISTANCE
+                        Minimum distance between barcodes. Default: 1
+  --homopolymer HOMOPOLYMER, -p HOMOPOLYMER
+                        Maximum homopolymer length. Default: 3
+  --levenshtein, -e     Use Levenshtein distance. Otherwise using Hamming diatnce. Default: False
+  --color, -c           Check optimal Illumina color balance. Default: False
+  --gc_min GC_MIN, -g GC_MIN
+                        Minimum GC content. Default: 0.4
+  --gc_max GC_MAX, -j GC_MAX
+                        Maximum GC content. Default: 0.6
+  --output OUTPUT, -o OUTPUT
+                        Output file. Default: STDOUT
+```
+
+```bash
+usage: monte sample [-h] --number NUMBER [--rejection-rate REJECTION_RATE] [--append APPEND] [--append_field APPEND_FIELD] [--distance DISTANCE] [--homopolymer HOMOPOLYMER] [--levenshtein] [--color]
+                    [--gc_min GC_MIN] [--gc_max GC_MAX] [--field FIELD] [--output OUTPUT]
+                    [input]
+
+positional arguments:
+  input                 Input file. Default: STDIN.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --number NUMBER, -n NUMBER
+                        Number of barcodes to generate. Required.
+  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
+                        Rate of rejection before aborting. Default: 0.85
+  --append APPEND       File to take a list of barcodes to extend. Default: do not use
+  --append_field APPEND_FIELD
+                        Column name or number to take barcodes from for appending. Default: 1
   --distance DISTANCE, -d DISTANCE
                         Minimum distance between barcodes. Default: 1
   --homopolymer HOMOPOLYMER, -p HOMOPOLYMER
                         Maximum homopolymer length. Default: 3
   --levenshtein, -e     Use Levenshtein distance. Otherwise using Hamming diatnce. Default: False
   --color, -c           Check optimal Illumina color balance. Default: False
   --gc_min GC_MIN, -g GC_MIN
                         Minimum GC content. Default: 0.4
   --gc_max GC_MAX, -j GC_MAX
                         Maximum GC content. Default: 0.6
+  --field FIELD, -f FIELD
+                        Column name or number for barcode sequences. Default: 1
   --output OUTPUT, -o OUTPUT
                         Output file. Default: STDOUT
 ```
 
 ```bash
 usage: monte check [-h] [--distance DISTANCE] [--homopolymer HOMOPOLYMER] [--levenshtein]
                    [--color] [--gc_min GC_MIN] [--gc_max GC_MAX] [--field FIELD] [--output OUTPUT]
@@ -356,8 +461,8 @@
 (Counter({'homopolymer': 1, 'palindrome': 1}), 4, ['ATCGCG', 'GCCGAT'])
 >>> mb.make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], n=1, checks=checks, quiet=True)
 (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG'])
 ```
 
 ### Documentation
 
-Full API documentation is [here](https://monte-barcode.readthedocs.org).
+Full API documentation is at [ReadTheDocs](https://monte-barcode.readthedocs.org).
```

### Comparing `monte-barcode-0.0.1.post1/README.md` & `monte-barcode-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # 🔴🟢🔵⚫️ monte barcode
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/scbirlab/monte-barcode/python-publish.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monte-barcode)
 ![PyPI](https://img.shields.io/pypi/v/monte-barcode)
 
 Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 
 ## Installation
 
@@ -28,15 +29,15 @@
 **monte barcode** provides command line utilities to generate completely random or 
 peptide-encoding barcodes conforming to custom contraints, like minimum edit
 distance among the set, GC content, and color balance for Illumina chemistry.
 
 Barcode sets and individual barcodes are deterministically given an adjective-noun mnemonic 
 (generated by [nemony](https://github.com/scbirlab/nemony)) for easy reference.
 
-Each utility gives a lot of commentary to `stderr`, but the barcodes go to
+Each utility writes a lot of commentary to `stderr`, but the barcodes go to
 `stdout` by default so they can be piped.
 
 ### Command line
 
 Generate random barcodes of a particular length.
 
 ```bash
@@ -129,14 +130,35 @@
 bright_cliff:l6-n10-d3:x6:oceanic_plume AGACTG
 bright_cliff:l6-n10-d3:x7:wanted_jessica        TCTCGA
 bright_cliff:l6-n10-d3:x8:incise_radical        TCTGTC
 bright_cliff:l6-n10-d3:x9:rebel_option  TAGGAC
 Wrote barcode set called bright_cliff, with minimum Hamming distance 3 and maximum Hamming distance 6.
 ```
 
+You can bias sampling based on a set of other sequences. This sampling conditions the choice of each base
+on the previous base.
+
+```bash
+$ monte barcode -n 5 --amino-acid HELP | monte sample --field 2 --distance 2 -n 5
+Generating barcodes with the following parameters:
+        ...
+Requested barcodes with length 12, and 16777216 possible combinations.
+> Tried 12 barcodes, rejected 7, accepted 5; rejection rate is 0.58
+
+Rejection reasons:
+        distance: 0.58
+        gc_content: 0.08
+ritzy_parker:l12-n5-d2:x0:good_race     CACGAATTGCCA
+ritzy_parker:l12-n5-d2:x1:wiry_cairo    CATGAACTACCA
+ritzy_parker:l12-n5-d2:x2:pricy_scuba   CACGAACTGCCT
+ritzy_parker:l12-n5-d2:x3:brisk_neptune CATGAATTGCCG
+ritzy_parker:l12-n5-d2:x4:dextrous_frame        CACGAATTACCG
+Wrote barcode set called ritzy_parker, with minimum Hamming distance 2 and maximum Hamming distance 3.
+```
+
 You can also check and filter previously generated sets.
 
 ```bash
 $ monte barcode --length 6 -n 10 -d 3 2> /dev/null | monte check --color --field 2
 Checking barcodes with the following parameters:
         ...
 > Tried 10 barcodes, rejected 6, accepted 4; rejection rate is 0.60
@@ -147,16 +169,46 @@
 thorough_adam:l6-n4-d4:x1:elfin_rufus   AGCTTC
 thorough_adam:l6-n4-d4:x2:damaged_atlas AAGGCA
 thorough_adam:l6-n4-d4:x3:faded_elite   GCACTA
 Wrote barcode set called thorough_adam, with minimum Hamming distance 4 and maximum Hamming distance 5.
 
 ```
 
-And try to sort by ideal color balance for Illumina chemistries (if you want to use subsets).
+Or use a previous set as a starting point for generating more, possibly with different parameters.
 
+```bash
+$ monte barcode -n10 --distance 4 --length 10  --append <(monte barcode -n 5 -a HELP) --append_field 2
+Generating barcodes with the following parameters:
+...
+> Tried 32 barcodes, rejected 22, accepted 10; rejection rate is 0.69
+
+Rejection reasons:
+        gc_content: 0.44
+        homopolymer: 0.47
+        distance: 0.03
+        palindrome: 0.03
+elegant_triton:l12-n15-d1:x0:vocal_stand        CACGAACTTCCT
+elegant_triton:l12-n15-d1:x1:real_clinic        CATGAATTGCCT
+elegant_triton:l12-n15-d1:x2:dextrous_frame     CACGAATTACCG
+elegant_triton:l12-n15-d1:x3:dizzy_record       CACGAATTACCT
+elegant_triton:l12-n15-d1:x4:prudent_jester     CACGAGCTACCA
+elegant_triton:l10-n15-d1:x5:useful_cabinet     ACGCGACACT
+elegant_triton:l10-n15-d1:x6:deafening_sphere   TAATACGCGC
+elegant_triton:l10-n15-d1:x7:old_program        ATCCTAAGCC
+elegant_triton:l10-n15-d1:x8:eager_doctor       TTGGCCACTG
+elegant_triton:l10-n15-d1:x9:dopey_limbo        ATCCGTCGTA
+elegant_triton:l10-n15-d1:x10:plain_lunar       ACGAGAATTC
+elegant_triton:l10-n15-d1:x11:discreet_ford     CTAACGTAGC
+elegant_triton:l10-n15-d1:x12:proud_jet CTTCAGTGTC
+elegant_triton:l10-n15-d1:x13:wry_insect        CAGACTGGAG
+elegant_triton:l10-n15-d1:x14:lofty_shave       TTCGTAACTC
+Wrote barcode set called elegant_triton, with minimum Hamming distance 1 and maximum Hamming distance 10.
+```
+
+And try to sort by ideal color balance for Illumina chemistries (if you want to use subsets).
 
 ```bash
 $ monte barcode --length 6 -n 15 -d 1 2> /dev/null | monte sort --field 2
 Sorting barcodes with the following parameters:
         ...
 round_mono:l6-n15-d2:x0:shady_soda      AGTCCT
 round_mono:l6-n15-d2:x1:vogue_cosmos    TGAGTC
@@ -175,39 +227,90 @@
 round_mono:l6-n15-d2:x14:discreet_shake GCATTG
 Wrote barcode set called round_mono, with minimum Hamming distance 2 and maximum Hamming distance 6.
 ```
 
 #### Details
 
 ```bash
-usage: monte barcode [-h] --number NUMBER [--length LENGTH] [--rejection-rate REJECTION_RATE]
-                     [--amino-acid AMINO_ACID] [--distance DISTANCE] [--homopolymer HOMOPOLYMER]
-                     [--levenshtein] [--color] [--gc_min GC_MIN] [--gc_max GC_MAX]
-                     [--output OUTPUT]
+usage: monte [-h] {barcode,check,sort,sample} ...
 
-options:
+Generate random DNA barcodes conforming to contraints, or check sets of barcodes for their conformance.
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+Sub-commands:
+  {barcode,check,sort,sample}
+                        Use these commands to specify the action you want.
+    barcode             Generate random barcodes.
+    check               Check barcode list.
+    sort                Sort barcode list for optimal color balance.
+    sample              Generate barcode list by sampling nucleotides from an existing list of sequences.
+```
+
+```bash
+usage: monte barcode [-h] [--length LENGTH] [--amino-acid AMINO_ACID] --number NUMBER [--rejection-rate REJECTION_RATE] [--append APPEND] [--append_field APPEND_FIELD] [--distance DISTANCE]
+                     [--homopolymer HOMOPOLYMER] [--levenshtein] [--color] [--gc_min GC_MIN] [--gc_max GC_MAX] [--output OUTPUT]
+
+optional arguments:
   -h, --help            show this help message and exit
-  --number NUMBER, -n NUMBER
-                        Number of barcodes to generate. Required.
   --length LENGTH, -l LENGTH
                         Barcode length. Default: 12
-  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
-                        Rate of rejection before aborting. Default: 0.85
   --amino-acid AMINO_ACID, -a AMINO_ACID
                         Generate barcodes encoding this amino acid sequence. Default: do not use.
+  --number NUMBER, -n NUMBER
+                        Number of barcodes to generate. Required.
+  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
+                        Rate of rejection before aborting. Default: 0.85
+  --append APPEND       File to take a list of barcodes to extend. Default: do not use
+  --append_field APPEND_FIELD
+                        Column name or number to take barcodes from for appending. Default: 1
+  --distance DISTANCE, -d DISTANCE
+                        Minimum distance between barcodes. Default: 1
+  --homopolymer HOMOPOLYMER, -p HOMOPOLYMER
+                        Maximum homopolymer length. Default: 3
+  --levenshtein, -e     Use Levenshtein distance. Otherwise using Hamming diatnce. Default: False
+  --color, -c           Check optimal Illumina color balance. Default: False
+  --gc_min GC_MIN, -g GC_MIN
+                        Minimum GC content. Default: 0.4
+  --gc_max GC_MAX, -j GC_MAX
+                        Maximum GC content. Default: 0.6
+  --output OUTPUT, -o OUTPUT
+                        Output file. Default: STDOUT
+```
+
+```bash
+usage: monte sample [-h] --number NUMBER [--rejection-rate REJECTION_RATE] [--append APPEND] [--append_field APPEND_FIELD] [--distance DISTANCE] [--homopolymer HOMOPOLYMER] [--levenshtein] [--color]
+                    [--gc_min GC_MIN] [--gc_max GC_MAX] [--field FIELD] [--output OUTPUT]
+                    [input]
+
+positional arguments:
+  input                 Input file. Default: STDIN.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --number NUMBER, -n NUMBER
+                        Number of barcodes to generate. Required.
+  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
+                        Rate of rejection before aborting. Default: 0.85
+  --append APPEND       File to take a list of barcodes to extend. Default: do not use
+  --append_field APPEND_FIELD
+                        Column name or number to take barcodes from for appending. Default: 1
   --distance DISTANCE, -d DISTANCE
                         Minimum distance between barcodes. Default: 1
   --homopolymer HOMOPOLYMER, -p HOMOPOLYMER
                         Maximum homopolymer length. Default: 3
   --levenshtein, -e     Use Levenshtein distance. Otherwise using Hamming diatnce. Default: False
   --color, -c           Check optimal Illumina color balance. Default: False
   --gc_min GC_MIN, -g GC_MIN
                         Minimum GC content. Default: 0.4
   --gc_max GC_MAX, -j GC_MAX
                         Maximum GC content. Default: 0.6
+  --field FIELD, -f FIELD
+                        Column name or number for barcode sequences. Default: 1
   --output OUTPUT, -o OUTPUT
                         Output file. Default: STDOUT
 ```
 
 ```bash
 usage: monte check [-h] [--distance DISTANCE] [--homopolymer HOMOPOLYMER] [--levenshtein]
                    [--color] [--gc_min GC_MIN] [--gc_max GC_MAX] [--field FIELD] [--output OUTPUT]
@@ -316,8 +419,8 @@
 (Counter({'homopolymer': 1, 'palindrome': 1}), 4, ['ATCGCG', 'GCCGAT'])
 >>> mb.make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], n=1, checks=checks, quiet=True)
 (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG'])
 ```
 
 ### Documentation
 
-Full API documentation is [here](https://monte-barcode.readthedocs.org).
+Full API documentation is at [ReadTheDocs](https://monte-barcode.readthedocs.org).
```

### Comparing `monte-barcode-0.0.1.post1/monte_barcode.egg-info/PKG-INFO` & `monte-barcode-0.0.2/monte_barcode.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monte-barcode
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,23 +27,26 @@
 Project-URL: Homepage, https://github.com/scbirlab/monte-barcode
 Project-URL: Bug Tracker, https://github.com/scbirlab/monte-barcode/issues
 Keywords: barcodes,sequencing,science,assay
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
 
 # 🔴🟢🔵⚫️ monte barcode
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/scbirlab/monte-barcode/python-publish.yml)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/monte-barcode)
 ![PyPI](https://img.shields.io/pypi/v/monte-barcode)
 
 Generating sets of random DNA sequences optimized for use in high-throughput sequencing.
 
 ## Installation
 
@@ -68,15 +71,15 @@
 **monte barcode** provides command line utilities to generate completely random or 
 peptide-encoding barcodes conforming to custom contraints, like minimum edit
 distance among the set, GC content, and color balance for Illumina chemistry.
 
 Barcode sets and individual barcodes are deterministically given an adjective-noun mnemonic 
 (generated by [nemony](https://github.com/scbirlab/nemony)) for easy reference.
 
-Each utility gives a lot of commentary to `stderr`, but the barcodes go to
+Each utility writes a lot of commentary to `stderr`, but the barcodes go to
 `stdout` by default so they can be piped.
 
 ### Command line
 
 Generate random barcodes of a particular length.
 
 ```bash
@@ -169,14 +172,35 @@
 bright_cliff:l6-n10-d3:x6:oceanic_plume AGACTG
 bright_cliff:l6-n10-d3:x7:wanted_jessica        TCTCGA
 bright_cliff:l6-n10-d3:x8:incise_radical        TCTGTC
 bright_cliff:l6-n10-d3:x9:rebel_option  TAGGAC
 Wrote barcode set called bright_cliff, with minimum Hamming distance 3 and maximum Hamming distance 6.
 ```
 
+You can bias sampling based on a set of other sequences. This sampling conditions the choice of each base
+on the previous base.
+
+```bash
+$ monte barcode -n 5 --amino-acid HELP | monte sample --field 2 --distance 2 -n 5
+Generating barcodes with the following parameters:
+        ...
+Requested barcodes with length 12, and 16777216 possible combinations.
+> Tried 12 barcodes, rejected 7, accepted 5; rejection rate is 0.58
+
+Rejection reasons:
+        distance: 0.58
+        gc_content: 0.08
+ritzy_parker:l12-n5-d2:x0:good_race     CACGAATTGCCA
+ritzy_parker:l12-n5-d2:x1:wiry_cairo    CATGAACTACCA
+ritzy_parker:l12-n5-d2:x2:pricy_scuba   CACGAACTGCCT
+ritzy_parker:l12-n5-d2:x3:brisk_neptune CATGAATTGCCG
+ritzy_parker:l12-n5-d2:x4:dextrous_frame        CACGAATTACCG
+Wrote barcode set called ritzy_parker, with minimum Hamming distance 2 and maximum Hamming distance 3.
+```
+
 You can also check and filter previously generated sets.
 
 ```bash
 $ monte barcode --length 6 -n 10 -d 3 2> /dev/null | monte check --color --field 2
 Checking barcodes with the following parameters:
         ...
 > Tried 10 barcodes, rejected 6, accepted 4; rejection rate is 0.60
@@ -187,16 +211,46 @@
 thorough_adam:l6-n4-d4:x1:elfin_rufus   AGCTTC
 thorough_adam:l6-n4-d4:x2:damaged_atlas AAGGCA
 thorough_adam:l6-n4-d4:x3:faded_elite   GCACTA
 Wrote barcode set called thorough_adam, with minimum Hamming distance 4 and maximum Hamming distance 5.
 
 ```
 
-And try to sort by ideal color balance for Illumina chemistries (if you want to use subsets).
+Or use a previous set as a starting point for generating more, possibly with different parameters.
 
+```bash
+$ monte barcode -n10 --distance 4 --length 10  --append <(monte barcode -n 5 -a HELP) --append_field 2
+Generating barcodes with the following parameters:
+...
+> Tried 32 barcodes, rejected 22, accepted 10; rejection rate is 0.69
+
+Rejection reasons:
+        gc_content: 0.44
+        homopolymer: 0.47
+        distance: 0.03
+        palindrome: 0.03
+elegant_triton:l12-n15-d1:x0:vocal_stand        CACGAACTTCCT
+elegant_triton:l12-n15-d1:x1:real_clinic        CATGAATTGCCT
+elegant_triton:l12-n15-d1:x2:dextrous_frame     CACGAATTACCG
+elegant_triton:l12-n15-d1:x3:dizzy_record       CACGAATTACCT
+elegant_triton:l12-n15-d1:x4:prudent_jester     CACGAGCTACCA
+elegant_triton:l10-n15-d1:x5:useful_cabinet     ACGCGACACT
+elegant_triton:l10-n15-d1:x6:deafening_sphere   TAATACGCGC
+elegant_triton:l10-n15-d1:x7:old_program        ATCCTAAGCC
+elegant_triton:l10-n15-d1:x8:eager_doctor       TTGGCCACTG
+elegant_triton:l10-n15-d1:x9:dopey_limbo        ATCCGTCGTA
+elegant_triton:l10-n15-d1:x10:plain_lunar       ACGAGAATTC
+elegant_triton:l10-n15-d1:x11:discreet_ford     CTAACGTAGC
+elegant_triton:l10-n15-d1:x12:proud_jet CTTCAGTGTC
+elegant_triton:l10-n15-d1:x13:wry_insect        CAGACTGGAG
+elegant_triton:l10-n15-d1:x14:lofty_shave       TTCGTAACTC
+Wrote barcode set called elegant_triton, with minimum Hamming distance 1 and maximum Hamming distance 10.
+```
+
+And try to sort by ideal color balance for Illumina chemistries (if you want to use subsets).
 
 ```bash
 $ monte barcode --length 6 -n 15 -d 1 2> /dev/null | monte sort --field 2
 Sorting barcodes with the following parameters:
         ...
 round_mono:l6-n15-d2:x0:shady_soda      AGTCCT
 round_mono:l6-n15-d2:x1:vogue_cosmos    TGAGTC
@@ -215,39 +269,90 @@
 round_mono:l6-n15-d2:x14:discreet_shake GCATTG
 Wrote barcode set called round_mono, with minimum Hamming distance 2 and maximum Hamming distance 6.
 ```
 
 #### Details
 
 ```bash
-usage: monte barcode [-h] --number NUMBER [--length LENGTH] [--rejection-rate REJECTION_RATE]
-                     [--amino-acid AMINO_ACID] [--distance DISTANCE] [--homopolymer HOMOPOLYMER]
-                     [--levenshtein] [--color] [--gc_min GC_MIN] [--gc_max GC_MAX]
-                     [--output OUTPUT]
+usage: monte [-h] {barcode,check,sort,sample} ...
 
-options:
+Generate random DNA barcodes conforming to contraints, or check sets of barcodes for their conformance.
+
+optional arguments:
+  -h, --help            show this help message and exit
+
+Sub-commands:
+  {barcode,check,sort,sample}
+                        Use these commands to specify the action you want.
+    barcode             Generate random barcodes.
+    check               Check barcode list.
+    sort                Sort barcode list for optimal color balance.
+    sample              Generate barcode list by sampling nucleotides from an existing list of sequences.
+```
+
+```bash
+usage: monte barcode [-h] [--length LENGTH] [--amino-acid AMINO_ACID] --number NUMBER [--rejection-rate REJECTION_RATE] [--append APPEND] [--append_field APPEND_FIELD] [--distance DISTANCE]
+                     [--homopolymer HOMOPOLYMER] [--levenshtein] [--color] [--gc_min GC_MIN] [--gc_max GC_MAX] [--output OUTPUT]
+
+optional arguments:
   -h, --help            show this help message and exit
-  --number NUMBER, -n NUMBER
-                        Number of barcodes to generate. Required.
   --length LENGTH, -l LENGTH
                         Barcode length. Default: 12
-  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
-                        Rate of rejection before aborting. Default: 0.85
   --amino-acid AMINO_ACID, -a AMINO_ACID
                         Generate barcodes encoding this amino acid sequence. Default: do not use.
+  --number NUMBER, -n NUMBER
+                        Number of barcodes to generate. Required.
+  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
+                        Rate of rejection before aborting. Default: 0.85
+  --append APPEND       File to take a list of barcodes to extend. Default: do not use
+  --append_field APPEND_FIELD
+                        Column name or number to take barcodes from for appending. Default: 1
+  --distance DISTANCE, -d DISTANCE
+                        Minimum distance between barcodes. Default: 1
+  --homopolymer HOMOPOLYMER, -p HOMOPOLYMER
+                        Maximum homopolymer length. Default: 3
+  --levenshtein, -e     Use Levenshtein distance. Otherwise using Hamming diatnce. Default: False
+  --color, -c           Check optimal Illumina color balance. Default: False
+  --gc_min GC_MIN, -g GC_MIN
+                        Minimum GC content. Default: 0.4
+  --gc_max GC_MAX, -j GC_MAX
+                        Maximum GC content. Default: 0.6
+  --output OUTPUT, -o OUTPUT
+                        Output file. Default: STDOUT
+```
+
+```bash
+usage: monte sample [-h] --number NUMBER [--rejection-rate REJECTION_RATE] [--append APPEND] [--append_field APPEND_FIELD] [--distance DISTANCE] [--homopolymer HOMOPOLYMER] [--levenshtein] [--color]
+                    [--gc_min GC_MIN] [--gc_max GC_MAX] [--field FIELD] [--output OUTPUT]
+                    [input]
+
+positional arguments:
+  input                 Input file. Default: STDIN.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --number NUMBER, -n NUMBER
+                        Number of barcodes to generate. Required.
+  --rejection-rate REJECTION_RATE, -r REJECTION_RATE
+                        Rate of rejection before aborting. Default: 0.85
+  --append APPEND       File to take a list of barcodes to extend. Default: do not use
+  --append_field APPEND_FIELD
+                        Column name or number to take barcodes from for appending. Default: 1
   --distance DISTANCE, -d DISTANCE
                         Minimum distance between barcodes. Default: 1
   --homopolymer HOMOPOLYMER, -p HOMOPOLYMER
                         Maximum homopolymer length. Default: 3
   --levenshtein, -e     Use Levenshtein distance. Otherwise using Hamming diatnce. Default: False
   --color, -c           Check optimal Illumina color balance. Default: False
   --gc_min GC_MIN, -g GC_MIN
                         Minimum GC content. Default: 0.4
   --gc_max GC_MAX, -j GC_MAX
                         Maximum GC content. Default: 0.6
+  --field FIELD, -f FIELD
+                        Column name or number for barcode sequences. Default: 1
   --output OUTPUT, -o OUTPUT
                         Output file. Default: STDOUT
 ```
 
 ```bash
 usage: monte check [-h] [--distance DISTANCE] [--homopolymer HOMOPOLYMER] [--levenshtein]
                    [--color] [--gc_min GC_MIN] [--gc_max GC_MAX] [--field FIELD] [--output OUTPUT]
@@ -356,8 +461,8 @@
 (Counter({'homopolymer': 1, 'palindrome': 1}), 4, ['ATCGCG', 'GCCGAT'])
 >>> mb.make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], n=1, checks=checks, quiet=True)
 (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG'])
 ```
 
 ### Documentation
 
-Full API documentation is [here](https://monte-barcode.readthedocs.org).
+Full API documentation is at [ReadTheDocs](https://monte-barcode.readthedocs.org).
```

### Comparing `monte-barcode-0.0.1.post1/montebarcode/checks.py` & `monte-barcode-0.0.2/montebarcode/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Functions to check that barcodes conform."""
 
+from __future__ import annotations
+
 from collections.abc import Callable, Iterable, Mapping, Sequence
 from collections import Counter, defaultdict
 from itertools import zip_longest
 import sys
 
 import streq as sq
 
-from .utils import pprint_dict
+from .utils import _print_err, pprint_dict
 
 
 def _print_rejection_reasons(x: Mapping, 
-                            n_tried: str) -> None:
+                             n_tried: str) -> None:
     
     key_val_str = {name: (s / n_tried) 
                    for name, s in x.items()}
 
     pprint_dict(key_val_str, '\nRejection reasons')
 
     return None
@@ -57,15 +59,18 @@
     
     dist_function = sq.levenshtein if use_levenshtein else sq.hamming
 
     all_distances = [dist_function(seq1, seq2) 
                      for i, seq1 in enumerate(x) 
                      for j, seq2 in enumerate(x) if i != j]
     
-    return min(all_distances), max(all_distances)
+    try:
+        return min(all_distances), max(all_distances)
+    except ValueError:
+        return 0, 0
         
 
 def Distance(min_distance: int = 2,
              use_levenshtein: bool = True) -> Callable[[str, Iterable], bool]:
     
     """Create a distance checking function.
 
@@ -444,36 +449,40 @@
 
 
 def make_checks(barcodes: Iterable[str],
                 n: int, 
                 checks: Iterable[Callable[[str, Sequence], bool]],
                 max_rejection_rate: float = 1.,
                 max_tries: int = 10000,
+                initial: Sequence[str] = None,
                 quiet: bool = False) -> Sequence[dict, int, Sequence[str]]:
     
     """Check barcode list conforms to the checks.
 
     Keeps a tally of rejection rate and rejection reasons.
 
     Parameters
     ----------
     barcodes : Iterable[str]
         List or generator of barcodes to check.
     n : int
-        Minimum number of barcodes to accept. Stops when this is reached.
+        Minimum number of barcodes to accept. Stops when this is reached or
+        checked all barcodes.
     checks : Iterable
         List of functions which take a candidate barcode and 
         previous barcodes as arguments and return True if the
         candidate should be rejected.
     length : int
         Length of barcodes to generate.
     max_rejection_rate : float, optional
         Rejection rate above which to terminate. Default: 1.
     max_tries : int, optional
         Number of barcodes to try before enforcing `max_rejection_rate`. Default 100000.
+    initial : list, optional
+        An initial list to append new barcodes. 
     quiet : bool, optional
         Whether to report progress. Default: True.
     
     Returns
     -------
     dict
         Counts of rejections based on failing each check.
@@ -497,18 +506,24 @@
     (Counter(), 4, ['AAAT', 'TCGC', 'ACAG', 'TGGC'])
     >>> # 
     >>> checks = [Homopolymer(), Palindrome()]
     >>> make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], 4, checks=checks, quiet=True)  # doctest: +NORMALIZE_WHITESPACE
     (Counter({'homopolymer': 1, 'palindrome': 1}), 4, ['ATCGCG', 'GCCGAT'])
     >>> make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], 1, checks=checks, quiet=True)  # doctest: +NORMALIZE_WHITESPACE
     (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG'])
+    >>> #
+    >>> make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], 1, checks=checks, initial=['ATCGCG'], quiet=True)   # doctest: +NORMALIZE_WHITESPACE
+    (Counter({'homopolymer': 1, 'palindrome': 1}), 3, ['ATCGCG', 'ATCGCG'])
+    >>> checks = [Homopolymer(), Palindrome(), Identities()] 
+    >>> make_checks(['AAAAT', 'CCCGGG', 'ATCGCG', 'GCCGAT'], 1, checks=checks, initial=['ATCGCG'], quiet=True)   # doctest: +NORMALIZE_WHITESPACE
+    (Counter({'homopolymer': 1, 'palindrome': 1, 'identity': 1}), 4, ['ATCGCG', 'GCCGAT'])
 
     """
     
-    accepted_barcodes = []
+    accepted_barcodes = initial or []
     fail_tally = Counter()
     n_tried, n_rejected, n_accepted = 0, 0, 0
     rejection_rate = 0.
 
     for i, new_barcode in enumerate(barcodes):
 
         n_tried = i + 1
@@ -532,23 +547,23 @@
                           f'threshold of {max_rejection_rate:.2f}')
                 
                 raise ValueError(message)
             
         else:
             
             accepted_barcodes.append(new_barcode)
-            n_accepted = len(accepted_barcodes)
+            n_accepted += 1
 
         rejection_rate =  n_rejected / n_tried
         
         if not quiet:
-            print(f'\r> Tried {n_tried} barcodes,',
-                f'rejected {n_rejected}, accepted {n_accepted};',
-                f'rejection rate is {rejection_rate:.2f}',
-                file=sys.stderr, end='')
+            _print_err(f'\r> Tried {n_tried} barcodes,',
+                       f'rejected {n_rejected}, accepted {n_accepted};',
+                       f'rejection rate is {rejection_rate:.2f}',
+                       end='')
         
         if n_accepted >= n:
 
             if not quiet:
                 print('', file=sys.stderr)
             break
```

### Comparing `monte-barcode-0.0.1.post1/montebarcode/cli.py` & `monte-barcode-0.0.2/montebarcode/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 """Command-line interface for monte-barcode."""
 
-from typing import TextIO
+from __future__ import annotations
+
+from typing import TextIO, Union
 from collections.abc import Callable, Mapping, Sequence
 import argparse
 import csv
 from functools import reduce
-from itertools import permutations
+from itertools import chain, permutations
 from math import factorial
 import operator
 import sys
 
 import nemony as nm
 import streq as sq
 from tqdm import tqdm
 
-from .generate import codon_barcodes, infinite_barcodes
+from .generate import codon_barcodes, infinite_barcodes, transition_matrix
 from . import checks
-from .utils import pprint_dict, _CODONS
-
+from .utils import _print_err, pprint_dict, _CODONS
 
 def _reader(input: TextIO, 
-            field: int) -> Sequence[str]:
+            field: Union[int, str]) -> Sequence[str]:
+
+    if field.isdigit():
+        infile = csv.reader(input, delimiter='\t')
+        key = int(field) - 1
+    else:
+        infile = csv.DictReader(input, delimiter='\t')
+        key = field
 
-    infile = csv.reader(input, delimiter='\t')
-    barcode_list = [row[field - 1] for row in infile]
+    barcode_list = [row[key] for row in infile]
     alphabet_used = set(letter for bc in barcode_list for letter in list(bc))
 
     assert all(letter in sq.sequences.DNA for letter in alphabet_used),\
                (f"ERROR: Letters other than {sq.sequences.DNA} are "
                 f"used in column {field} of {input.name}")
     
     return barcode_list
@@ -39,39 +46,40 @@
 
     barcode_set_name = nm.encode(barcodes)
 
     outfile = csv.writer(output, 
                          delimiter='\t')
     min_distance, max_distance = checks.minmax_distance(barcodes, levenshtein)
     n = len(barcodes)
-    
+
     try:
 
         for i, barcode in enumerate(barcodes):
+
             row = (f'{barcode_set_name}:'
                    f'l{len(barcode)}-n{n}-d{min_distance}:'
                    f'x{i}:{nm.encode(barcode)}'), barcode
             outfile.writerow(row)
 
     except BrokenPipeError:
 
         pass
 
     distance = 'Levenshtein' if levenshtein else 'Hamming'
         
-    print(f'Wrote barcode set called {barcode_set_name},',
-          f'with minimum {distance} distance {min_distance} and',
-          f'maximum {distance} distance {max_distance}.', 
-          file=sys.stderr)
+    _print_err(f'Wrote barcode set called {barcode_set_name},',
+               f'with minimum {distance} distance {min_distance} and',
+               f'maximum {distance} distance {max_distance}.')
     
     return None
 
 
 def _checker(args: argparse.Namespace, 
-             barcode_list: Sequence[str]) -> Sequence[str]:
+             barcode_list: Sequence[str],
+             initial: Sequence[str] = []) -> Sequence[str]:
 
     checklist = [checks.Identities(), 
                  checks.Palindrome(),
                  checks.Distance(min_distance=args.distance,
                                  use_levenshtein=args.levenshtein),
                  checks.GCcontent(min=args.gc_min, 
                                   max=args.gc_max),
@@ -84,25 +92,26 @@
     try:
         n = len(barcode_list)
         max_rejection_rate = 1.
     except TypeError:
         n = args.number
         max_rejection_rate = args.rejection_rate
 
-    _, _, barcodes = checks.make_checks(barcode_list,
-                                 n=n, 
-                                 max_rejection_rate=max_rejection_rate,
-                                 checks=checklist)
+    (_, _, 
+     barcodes) = checks.make_checks(barcode_list,
+                                    n=n, 
+                                    max_rejection_rate=max_rejection_rate,
+                                    checks=checklist,
+                                    initial=initial)
     
     if len(barcodes) < n:
 
-        print(f'Could only generate {len(barcodes)} barcodes,',
-              f'but {n} were requested.',
-              'You might need to try different settings.',
-              file=sys.stderr)
+        _print_err(f'WARNING: Could only generate {len(barcodes)} barcodes,',
+                   f'but {n} were requested.',
+                   'You might need to try different settings.')
     
     _writer(args.output, barcodes, args.levenshtein)
 
     return barcodes
 
 
 def _check_permutations(barcodes: Sequence[str], 
@@ -116,20 +125,21 @@
    
     result = None
 
     for permutation in tqdm(permutations(barcodes, n), 
                             total=n_permutations):
 
         try:
-            fail_tally, _, result = checks.make_checks(constant + list(permutation),
-                                                n=len(permutation),
-                                                max_rejection_rate=0.,
-                                                checks=checklist,
-                                                max_tries=0,
-                                                quiet=True)
+            (fail_tally, _, 
+             result) = checks.make_checks(constant + list(permutation),
+                                          n=len(permutation),
+                                          max_rejection_rate=0.,
+                                          checks=checklist,
+                                          max_tries=0,
+                                          quiet=True)
         except ValueError:
 
             pass
 
         else:
 
             break
@@ -149,38 +159,36 @@
     barcode_list = _reader(args.input, args.field)
     
     checklist = [checks.IlluminaColorBalance()]
 
     try:
         
         _, _, barcodes = checks.make_checks(barcode_list,
-                                              n=len(barcode_list),
-                                              max_rejection_rate=0.,
-                                              checks=checklist,
-                                              max_tries=0,
-                                              quiet=True)
+                                            n=len(barcode_list),
+                                            max_rejection_rate=0.,
+                                            checks=checklist,
+                                            max_tries=0,
+                                            quiet=True)
         
     except ValueError:
         
         _, starter_barcodes = _check_permutations(barcode_list, 
                                                   checklist, n=6)
         remaining_barcodes = list(set(barcode_list) - 
                                   set(starter_barcodes))
 
         _, barcodes = _check_permutations(remaining_barcodes, 
                                           checklist,
                                           constant=list(starter_barcodes))
-        # barcodes = list(starter_barcodes) + list(barcodes)
 
     if len(barcodes) < len(barcode_list):
 
-        print(f'Could only generate {len(barcodes)} barcodes,',
-              f'but {len(barcode_list)} were provided.',
-              'You might need to try different settings.',
-              file=sys.stderr)
+        _print_err(f'Could only generate {len(barcodes)} barcodes,',
+                   f'but {len(barcode_list)} were provided.',
+                   'You might need to try different settings.')
 
     _writer(args.output, barcodes)
     
     return None
 
 
 def check_barcodes(args: argparse.Namespace) -> None:
@@ -196,45 +204,71 @@
 
 
 def generate(args: argparse.Namespace) -> None:
 
     pprint_dict(vars(args), 
                 'Generating barcodes with the following parameters')
     
-    if args.amino_acid is not None:
+    if args.subcommand != 'sample' and args.amino_acid is not None:
 
         invalid_aa = [aa for aa in args.amino_acid if aa not in _CODONS]
 
-        assert len(invalid_aa) == 0, "The following amino acids are invalid: {}".format(", ".join(invalid_aa))
+        assert len(invalid_aa) == 0, \
+            "The following amino acids are invalid: {}".format(", ".join(invalid_aa))
 
         length = len(args.amino_acid) * 3
         combinations = reduce(operator.mul, (len(_CODONS[aa]) for aa in args.amino_acid))
-        print(f'Using amino acid sequence {args.amino_acid} with',
-              f'length {length} and {combinations} possible combinations.',
-              file=sys.stderr)
+        
+        _print_err(f'Using amino acid sequence {args.amino_acid} with',
+                   f'length {length} and {combinations} possible combinations.')
         
         barcodes = codon_barcodes(args.amino_acid)
 
     else:
 
-        length = args.length
-        alphabet_length = len(sq.sequences.DNA)
-        combinations = alphabet_length ** args.length
-
-        print(f'Requested barcodes with length {length},',
-              f'and {combinations} possible combinations.',
-              file=sys.stderr)
+        if args.subcommand == 'sample':
+
+            barcode_list = _reader(args.input, args.field)
+            alphabet = transition_matrix(barcode_list)
+            length = len(alphabet)
+            alphabet_length = len(list(set(chain(*barcode_list))))
+            check_used = False
+            # TODO: Currently is an upper limit; make accurate.
+            combinations = reduce(operator.mul, 
+                                  (max(len(letters) for _, (letters, _) in position.items()) 
+                                   for position in alphabet))
+        else:
+
+            length = args.length
+            alphabet = sq.sequences.DNA
+            alphabet_length = len(alphabet)
+            check_used = True
+            combinations = alphabet_length ** length
+
+        _print_err(f'Requested barcodes with length {length},',
+                   f'and {combinations} possible combinations.')
+        
+        barcodes = infinite_barcodes(length,
+                                     alphabet=alphabet,
+                                     check_used=check_used)
         
-        barcodes = infinite_barcodes(length)
+    if args.append is not None:
+
+        initial = _reader(args.append, args.append_field)
+
+    else:
+
+        initial = []
     
     assert combinations > args.number,\
             f'There are not {args.number} unique {length}-mers. '\
-            f'Maximum is {combinations}.'
+            f'Maximum is {combinations}. You might need to try'\
+            'different settings.'
 
-    barcodes = _checker(args, barcodes)
+    barcodes = _checker(args, barcodes, initial=initial)
 
     return None
     
 
 def main() -> None:
 
     parser = argparse.ArgumentParser(description='''
@@ -251,30 +285,45 @@
     barcode.set_defaults(func=generate)
     check = subcommands.add_parser('check', 
                                     help='Check barcode list.')
     check.set_defaults(func=check_barcodes)
     sort = subcommands.add_parser('sort', 
                                   help='Sort barcode list for optimal color balance.')
     sort.set_defaults(func=sort_barcodes)
-    
-    barcode.add_argument('--number', '-n', 
-                         type=int, required=True,
-                         help='Number of barcodes to generate. Required.')
+    sample = subcommands.add_parser('sample', 
+                                    help='Generate barcode list by sampling nucleotides '
+                                         'from an existing list of sequences.')
+    sample.set_defaults(func=generate)
+   
     barcode.add_argument('--length', '-l', 
                          type=int, default=12,
                          help='Barcode length. Default: %(default)s')
-    barcode.add_argument('--rejection-rate', '-r', 
-                         type=float, default=.85,
-                         help='Rate of rejection before aborting. Default: %(default)s')
     barcode.add_argument('--amino-acid', '-a', 
                          type=str, 
                          default=None,
                          help='Generate barcodes encoding this amino acid sequence. Default: do not use.')
     
-    for p in (barcode, check):
+    for p in (barcode, sample):
+
+        p.add_argument('--number', '-n', 
+                       type=int, required=True,
+                       help='Number of barcodes to generate. Required.')
+        p.add_argument('--rejection-rate', '-r', 
+                       type=float, default=.85,
+                       help='Rate of rejection before aborting. Default: %(default)s')
+        p.add_argument('--append', 
+                       type=argparse.FileType('r'), 
+                       default=None,
+                       help='File to take a list of barcodes to extend. Default: do not use')
+        p.add_argument('--append_field', 
+                       type=str, 
+                       default='1',
+                       help='Column name or number to take barcodes from for appending. Default: %(default)s')
+    
+    for p in (barcode, check, sample):
     
         p.add_argument('--distance', '-d', 
                        type=int, default=1,
                        help='Minimum distance between barcodes. Default: %(default)s')
         p.add_argument('--homopolymer', '-p', 
                        type=int, default=3,
                        help='Maximum homopolymer length. Default: %(default)s')
@@ -288,27 +337,27 @@
         p.add_argument('--gc_min', '-g', 
                        type=float, default=.4,
                        help='Minimum GC content. Default: %(default)s')
         p.add_argument('--gc_max', '-j', 
                        type=float, default=.6,
                        help='Maximum GC content. Default: %(default)s')
         
-    for p in (check, sort):
+    for p in (check, sort, sample):
 
         p.add_argument('input',
-                    type=argparse.FileType('r'),
-                    nargs='?',
-                    default=sys.stdin,
-                    help='Input file. Default: STDIN.')
+                       type=argparse.FileType('r'),
+                       nargs='?',
+                       default=sys.stdin,
+                       help='Input file. Default: STDIN.')
         p.add_argument('--field', '-f',
-                    type=int,
-                    default=1,
-                    help='Column number for barcode sequences. Default: %(default)s')
+                       type=str,
+                       default='1',
+                       help='Column name or number for barcode sequences. Default: %(default)s')
         
-    for p in (barcode, check, sort):
+    for p in (barcode, check, sort, sample):
 
         p.add_argument('--output', '-o', 
                        type=argparse.FileType('w'),
                        default=sys.stdout,
                        help='Output file. Default: STDOUT')
         
     args = parser.parse_args()
```

### Comparing `monte-barcode-0.0.1.post1/pyproject.toml` & `monte-barcode-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [project]
 name = "monte-barcode"
-version = "0.0.1post1"
+version = "0.0.2"
 authors = [
   { name="Eachan Johnson", email="eachan.johnson@crick.ac.uk" },
 ]
 description = "Generating sets of random DNA sequences optimized for use in high-throughput sequencing."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["barcodes", "sequencing", "science", "assay"]
 
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
-  "streq",
-  "nemony",
+  "streq>=0.0.2",
+  "nemony>=0.0.2",
   "tqdm",
   "pyyaml"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/scbirlab/monte-barcode"
 "Bug Tracker" = "https://github.com/scbirlab/monte-barcode/issues"
```

