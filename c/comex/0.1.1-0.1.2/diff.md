# Comparing `tmp/comex-0.1.1.tar.gz` & `tmp/comex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.1.1.tar", last modified: Thu Jun  1 12:42:45 2023, max compression
+gzip compressed data, was "comex-0.1.2.tar", last modified: Fri Jun  2 11:56:52 2023, max compression
```

## Comparing `comex-0.1.1.tar` & `comex-0.1.2.tar`

### file list

```diff
@@ -1,60 +1,58 @@
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.915888 comex-0.1.1/
--rw-r--r--   0 noble      (501) staff       (20)    11357 2023-06-01 12:38:00.000000 comex-0.1.1/LICENSE
--rw-r--r--   0 noble      (501) staff       (20)     8209 2023-06-01 12:42:45.915991 comex-0.1.1/PKG-INFO
--rw-r--r--   0 noble      (501) staff       (20)     7592 2023-06-01 12:38:00.000000 comex-0.1.1/README.md
--rw-r--r--   0 noble      (501) staff       (20)     1036 2023-06-01 12:42:45.916386 comex-0.1.1/setup.cfg
--rw-r--r--   0 noble      (501) staff       (20)       38 2023-06-01 12:38:00.000000 comex-0.1.1/setup.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.908534 comex-0.1.1/src/
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.910353 comex-0.1.1/src/comex/
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/__init__.py
--rw-r--r--   0 noble      (501) staff       (20)      104 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/__main__.py
--rw-r--r--   0 noble      (501) staff       (20)     3664 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/cli.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.911340 comex-0.1.1/src/comex/codeviews/
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.911731 comex-0.1.1/src/comex/codeviews/AST/
--rw-r--r--   0 noble      (501) staff       (20)     4196 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/AST/AST.py
--rw-r--r--   0 noble      (501) staff       (20)      968 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/AST/AST_driver.py
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/AST/__init__.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.912689 comex-0.1.1/src/comex/codeviews/CFG/
--rw-r--r--   0 noble      (501) staff       (20)     1426 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG.py
--rw-r--r--   0 noble      (501) staff       (20)    51528 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG_csharp.py
--rw-r--r--   0 noble      (501) staff       (20)     1300 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG_driver.py
--rw-r--r--   0 noble      (501) staff       (20)    78323 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG_java.py
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/__init__.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.913002 comex-0.1.1/src/comex/codeviews/CST/
--rw-r--r--   0 noble      (501) staff       (20)     2540 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CST/CST_driver.py
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CST/__init__.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.913297 comex-0.1.1/src/comex/codeviews/DFG/
--rw-r--r--   0 noble      (501) staff       (20)     1246 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/DFG/DFG_driver.py
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/DFG/__init__.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.913865 comex-0.1.1/src/comex/codeviews/SDFG/
--rw-r--r--   0 noble      (501) staff       (20)     4535 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/SDFG.py
--rw-r--r--   0 noble      (501) staff       (20)    32117 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/SDFG_csharp.py
--rw-r--r--   0 noble      (501) staff       (20)    61608 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/SDFG_java.py
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/__init__.py
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/__init__.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.914083 comex-0.1.1/src/comex/codeviews/combined_graph/
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/combined_graph/__init__.py
--rw-r--r--   0 noble      (501) staff       (20)     9551 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/combined_graph/combined_driver.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.914705 comex-0.1.1/src/comex/tree_parser/
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/__init__.py
--rw-r--r--   0 noble      (501) staff       (20)     8617 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/cs_parser.py
--rw-r--r--   0 noble      (501) staff       (20)     6152 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/custom_parser.py
--rw-r--r--   0 noble      (501) staff       (20)    10057 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/java_parser.py
--rw-r--r--   0 noble      (501) staff       (20)     1818 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/parser_driver.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.915630 comex-0.1.1/src/comex/utils/
--rw-r--r--   0 noble      (501) staff       (20)     1763 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/DFG_utils.py
--rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/__init__.py
--rw-r--r--   0 noble      (501) staff       (20)    19424 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/cs_nodes.py
--rw-r--r--   0 noble      (501) staff       (20)    25191 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/java_nodes.py
--rw-r--r--   0 noble      (501) staff       (20)     1083 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/postprocessor.py
--rw-r--r--   0 noble      (501) staff       (20)     2418 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/preprocessor.py
--rw-r--r--   0 noble      (501) staff       (20)     2055 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/src_parser.py
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.911200 comex-0.1.1/src/comex.egg-info/
--rw-r--r--   0 noble      (501) staff       (20)     8209 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/PKG-INFO
--rw-r--r--   0 noble      (501) staff       (20)     1428 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/SOURCES.txt
--rw-r--r--   0 noble      (501) staff       (20)        1 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/dependency_links.txt
--rw-r--r--   0 noble      (501) staff       (20)       40 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/entry_points.txt
--rw-r--r--   0 noble      (501) staff       (20)      151 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/requires.txt
--rw-r--r--   0 noble      (501) staff       (20)        6 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/top_level.txt
-drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.915770 comex-0.1.1/tests/
--rw-r--r--   0 noble      (501) staff       (20)     4508 2023-06-01 12:38:00.000000 comex-0.1.1/tests/test_codeviews.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-27 09:03:42.000000 comex-0.1.2/LICENSE
+-rwxrwxrwx   0 noble      (501) staff       (20)    11440 2023-06-02 11:56:52.920000 comex-0.1.2/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)    10823 2023-06-02 07:57:13.000000 comex-0.1.2/README.md
+-rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-06-02 11:56:52.920000 comex-0.1.2/setup.cfg
+-rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-27 09:03:43.000000 comex-0.1.2/setup.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      104 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/__main__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     3664 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/cli.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/AST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4196 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/codeviews/AST/AST.py
+-rwxrwxrwx   0 noble      (501) staff       (20)      968 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/AST/AST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/AST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/CFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1426 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    51528 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1300 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    78323 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/CFG/CFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/CST/
+-rwxrwxrwx   0 noble      (501) staff       (20)     2540 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CST/CST_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/CST/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/DFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1246 2023-05-31 12:50:30.000000 comex-0.1.2/src/comex/codeviews/DFG/DFG_driver.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/DFG/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/SDFG/
+-rwxrwxrwx   0 noble      (501) staff       (20)     4535 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/SDFG/SDFG.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    32117 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/codeviews/SDFG/SDFG_csharp.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    61608 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/SDFG/SDFG_java.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/SDFG/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/__init__.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/codeviews/combined_graph/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/combined_graph/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     9551 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/codeviews/combined_graph/combined_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/tree_parser/
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/tree_parser/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     8617 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/tree_parser/cs_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     6152 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/tree_parser/custom_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    10057 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/tree_parser/java_parser.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1818 2023-05-29 09:20:48.000000 comex-0.1.2/src/comex/tree_parser/parser_driver.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex/utils/
+-rwxrwxrwx   0 noble      (501) staff       (20)     1763 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/utils/DFG_utils.py
+-rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 09:07:09.000000 comex-0.1.2/src/comex/utils/__init__.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    19424 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/utils/cs_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)    25191 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/utils/java_nodes.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     1083 2023-06-02 04:07:10.000000 comex-0.1.2/src/comex/utils/postprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2418 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/utils/preprocessor.py
+-rwxrwxrwx   0 noble      (501) staff       (20)     2055 2023-05-27 09:03:43.000000 comex-0.1.2/src/comex/utils/src_parser.py
+drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-06-02 11:56:52.900000 comex-0.1.2/src/comex.egg-info/
+-rwxrwxrwx   0 noble      (501) staff       (20)    11440 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/PKG-INFO
+-rwxrwxrwx   0 noble      (501) staff       (20)     1404 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/SOURCES.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/dependency_links.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/entry_points.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/requires.txt
+-rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-06-02 11:56:52.000000 comex-0.1.2/src/comex.egg-info/top_level.txt
```

### Comparing `comex-0.1.1/LICENSE` & `comex-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/PKG-INFO` & `comex-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: comex
-Version: 0.1.1
-Summary: Generate combined multi-code view graphs
-Home-page: https://github.com/IBM/tree-sitter-codeviews
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Tree Sitter Multi Codeview Generator
 
 Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
 # Comex
 `comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
@@ -84,20 +67,144 @@
 output_file: denotes the output file to which the generated graph is written
 
 graph_format: denotes the format of the output graph. Currently supported formats are "dot" and "json". To generate both pass "all"
 
 codeviews: refers to the configuration passed for each codeview
 ````
 
-### Output Example:
+### Output Examples:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
-<img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
+![Sample AST CFG DFG](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/sample.png)
+
+Below we present more examples of input code snippets and generated codeviews for both Java and C#.
+
+---
+
+**CLI Command**:
+
+```bash
+comex --lang "java" --code-file sample/example.java --graphs "cfg,dfg"
+```
+---
+
+**Java Code Snippet**:
+
+```Java
+import java.io.ByteArrayInputStream;
+import java.io.InputStream;
+import java.util.ArrayList;
+import java.util.List;
+import java.util.Scanner;
+
+public class Main {
+    //    static String INPUT = "5\n3 2 2 4 1\n1 2 2 2 1";
+    static String INPUT = "";
+
+    public static void main(String[] args) {
+        InputStream is = INPUT.isEmpty() ? System.in : new ByteArrayInputStream(INPUT.getBytes());
+
+        Scanner scanner = new Scanner(is);
+
+        final int n = scanner.nextInt();
+        List<Position> positionList = new ArrayList<>(n);
+        for (int i = 0; i < n; i++) {
+            positionList.add(
+                    new Position(
+                            scanner.nextInt(),
+                            scanner.nextInt(),
+                            scanner.nextInt()
+                    )
+            );
+        }
+
+        System.out.println(solve(positionList) ? "Yes" : "No");
+    }
+
+    static class Position {
+        int t;
+        int x;
+        int y;
+
+        public Position(int t, int x, int y) {
+            this.t = t;
+            this.x = x;
+            this.y = y;
+        }
+    }
+
+    static boolean solve(List<Position> positionList) {
+        Position currentPosition = new Position(0, 0, 0);
+        for (int i = 0; i < positionList.size(); i++) {
+            Position nextPosition = positionList.get(i);
+            if (!possibleMove(currentPosition.t, nextPosition.t, currentPosition.x, nextPosition.x, currentPosition.y, nextPosition.y)) {
+                return false;
+            }
+            currentPosition = nextPosition;
+        }
+        return true;
+    }
+
+    static boolean possibleMove(int t1, int t2, int x1, int x2, int y1, int y2) {
+        int tDiff = t2 - t1;
+        int absX = Math.abs(x1 - x2);
+        int absY = Math.abs(y1 - y2);
+
+        if (absX + absY <= tDiff) {
+            if (tDiff % 2 == (absX + absY) % 2) {
+                return true;
+            }
+        }
+        return false;
+    }
+
+}
+
+```
+---
+
+**Generated Codeview**:
+
+![Java File-level](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/java.png)
+
+---
+
+**CLI Command**:
+
+```bash
+comex --lang "cs" --code-file sample/example.cs --graphs "cfg,dfg"
+```
+---
+
+**C# Code Snippet**:
+
+```C#
+public class DFG_A2 {
+    public void main(string[] args) {
+        BufferedReader br = new BufferedReader(new InputStreamReader(System.in)); // {}
+        String str = br.attribute1; // {3}
+        str = br.attribute2.method1(); // {3}
+        br.attribute1 = br.attribute2; // {3,5}
+        br.method2(br.attribute1, br.attribute2); // {3,5,6}
+        BufferedReader br2 = br; // {5,6,7}
+        br.method3(); // {5,6,7}
+        int j = br2.attribute1.method2(3,4); // {8}
+    }
+}
+```
+---
+
+**Generated Codeview**:
+
+![C# Method-level](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/cs.png)
+
+---
 
+More examples and results can be found in the [tests/data](https://github.com/IBM/tree-sitter-codeviews/tree/main/tests/data) directory
 
 ### Code Organization
 The code is structured in the following way:
 1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
 2. The [codeviews](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
 3. The [cli.py](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
```

### Comparing `comex-0.1.1/setup.cfg` & `comex-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.1.1
+version = 0.1.2
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.1.1/src/comex/cli.py` & `comex-0.1.2/src/comex/cli.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/AST/AST.py` & `comex-0.1.2/src/comex/codeviews/AST/AST.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/AST/AST_driver.py` & `comex-0.1.2/src/comex/codeviews/AST/AST_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/CFG/CFG.py` & `comex-0.1.2/src/comex/codeviews/CFG/CFG.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/CFG/CFG_csharp.py` & `comex-0.1.2/src/comex/codeviews/CFG/CFG_csharp.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/CFG/CFG_driver.py` & `comex-0.1.2/src/comex/codeviews/CFG/CFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/CFG/CFG_java.py` & `comex-0.1.2/src/comex/codeviews/CFG/CFG_java.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/CST/CST_driver.py` & `comex-0.1.2/src/comex/codeviews/CST/CST_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/DFG/DFG_driver.py` & `comex-0.1.2/src/comex/codeviews/DFG/DFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/SDFG/SDFG.py` & `comex-0.1.2/src/comex/codeviews/SDFG/SDFG.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/SDFG/SDFG_csharp.py` & `comex-0.1.2/src/comex/codeviews/SDFG/SDFG_csharp.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/SDFG/SDFG_java.py` & `comex-0.1.2/src/comex/codeviews/SDFG/SDFG_java.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/codeviews/combined_graph/combined_driver.py` & `comex-0.1.2/src/comex/codeviews/combined_graph/combined_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/tree_parser/cs_parser.py` & `comex-0.1.2/src/comex/tree_parser/cs_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/tree_parser/custom_parser.py` & `comex-0.1.2/src/comex/tree_parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/tree_parser/java_parser.py` & `comex-0.1.2/src/comex/tree_parser/java_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/tree_parser/parser_driver.py` & `comex-0.1.2/src/comex/tree_parser/parser_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/utils/DFG_utils.py` & `comex-0.1.2/src/comex/utils/DFG_utils.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/utils/cs_nodes.py` & `comex-0.1.2/src/comex/utils/cs_nodes.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/utils/java_nodes.py` & `comex-0.1.2/src/comex/utils/java_nodes.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/utils/postprocessor.py` & `comex-0.1.2/src/comex/utils/postprocessor.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/utils/preprocessor.py` & `comex-0.1.2/src/comex/utils/preprocessor.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex/utils/src_parser.py` & `comex-0.1.2/src/comex/utils/src_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.1/src/comex.egg-info/PKG-INFO` & `comex-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -84,20 +84,144 @@
 output_file: denotes the output file to which the generated graph is written
 
 graph_format: denotes the format of the output graph. Currently supported formats are "dot" and "json". To generate both pass "all"
 
 codeviews: refers to the configuration passed for each codeview
 ````
 
-### Output Example:
+### Output Examples:
 
 Combined simple AST+CFG+DFG for a simple Java program that finds the maximum among 2 numbers:
 
-<img src="https://github.com/IBM/tree-sitter-codeviews/raw/main/sample.png" >
+![Sample AST CFG DFG](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/sample.png)
 
+Below we present more examples of input code snippets and generated codeviews for both Java and C#.
+
+---
+
+**CLI Command**:
+
+```bash
+comex --lang "java" --code-file sample/example.java --graphs "cfg,dfg"
+```
+---
+
+**Java Code Snippet**:
+
+```Java
+import java.io.ByteArrayInputStream;
+import java.io.InputStream;
+import java.util.ArrayList;
+import java.util.List;
+import java.util.Scanner;
+
+public class Main {
+    //    static String INPUT = "5\n3 2 2 4 1\n1 2 2 2 1";
+    static String INPUT = "";
+
+    public static void main(String[] args) {
+        InputStream is = INPUT.isEmpty() ? System.in : new ByteArrayInputStream(INPUT.getBytes());
+
+        Scanner scanner = new Scanner(is);
+
+        final int n = scanner.nextInt();
+        List<Position> positionList = new ArrayList<>(n);
+        for (int i = 0; i < n; i++) {
+            positionList.add(
+                    new Position(
+                            scanner.nextInt(),
+                            scanner.nextInt(),
+                            scanner.nextInt()
+                    )
+            );
+        }
+
+        System.out.println(solve(positionList) ? "Yes" : "No");
+    }
+
+    static class Position {
+        int t;
+        int x;
+        int y;
+
+        public Position(int t, int x, int y) {
+            this.t = t;
+            this.x = x;
+            this.y = y;
+        }
+    }
+
+    static boolean solve(List<Position> positionList) {
+        Position currentPosition = new Position(0, 0, 0);
+        for (int i = 0; i < positionList.size(); i++) {
+            Position nextPosition = positionList.get(i);
+            if (!possibleMove(currentPosition.t, nextPosition.t, currentPosition.x, nextPosition.x, currentPosition.y, nextPosition.y)) {
+                return false;
+            }
+            currentPosition = nextPosition;
+        }
+        return true;
+    }
+
+    static boolean possibleMove(int t1, int t2, int x1, int x2, int y1, int y2) {
+        int tDiff = t2 - t1;
+        int absX = Math.abs(x1 - x2);
+        int absY = Math.abs(y1 - y2);
+
+        if (absX + absY <= tDiff) {
+            if (tDiff % 2 == (absX + absY) % 2) {
+                return true;
+            }
+        }
+        return false;
+    }
+
+}
+
+```
+---
+
+**Generated Codeview**:
+
+![Java File-level](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/java.png)
+
+---
+
+**CLI Command**:
+
+```bash
+comex --lang "cs" --code-file sample/example.cs --graphs "cfg,dfg"
+```
+---
+
+**C# Code Snippet**:
+
+```C#
+public class DFG_A2 {
+    public void main(string[] args) {
+        BufferedReader br = new BufferedReader(new InputStreamReader(System.in)); // {}
+        String str = br.attribute1; // {3}
+        str = br.attribute2.method1(); // {3}
+        br.attribute1 = br.attribute2; // {3,5}
+        br.method2(br.attribute1, br.attribute2); // {3,5,6}
+        BufferedReader br2 = br; // {5,6,7}
+        br.method3(); // {5,6,7}
+        int j = br2.attribute1.method2(3,4); // {8}
+    }
+}
+```
+---
+
+**Generated Codeview**:
+
+![C# Method-level](https://github.com/IBM/tree-sitter-codeviews/raw/main/sample/cs.png)
+
+---
+
+More examples and results can be found in the [tests/data](https://github.com/IBM/tree-sitter-codeviews/tree/main/tests/data) directory
 
 ### Code Organization
 The code is structured in the following way:
 1. For each code-view, first the source code is parsed using the tree-sitter parser and then the various code-views are generated. In the [tree_parser](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/tree_parser) directory, the Parser and ParserDriver is implemented with various funcitonalities commonly required by all code-views. Language-specific features are further developed in the language-specific parsers also placed in this directory.
 2. The [codeviews](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/codeviews) directory contains the core logic for the various codeviews. Each codeview has a driver class and a codeview class, which is further inherited and extended by language in case of code-views that require language-specific implementation.
 3. The [cli.py](https://github.com/IBM/tree-sitter-codeviews/tree/main/src/comex/cli.py) file is the CLI implementation. The drivers can also be directly imported and used like a python package. It is responsible for parsing the source code and generating the codeviews.
```

### Comparing `comex-0.1.1/src/comex.egg-info/SOURCES.txt` & `comex-0.1.2/src/comex.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,9 +37,8 @@
 src/comex/tree_parser/parser_driver.py
 src/comex/utils/DFG_utils.py
 src/comex/utils/__init__.py
 src/comex/utils/cs_nodes.py
 src/comex/utils/java_nodes.py
 src/comex/utils/postprocessor.py
 src/comex/utils/preprocessor.py
-src/comex/utils/src_parser.py
-tests/test_codeviews.py
+src/comex/utils/src_parser.py
```

