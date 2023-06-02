# Comparing `tmp/enforce_notebook_run_order-0.1.2.tar.gz` & `tmp/enforce_notebook_run_order-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-0.1.2.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-0.1.3.tar", max compression
```

## Comparing `enforce_notebook_run_order-0.1.2.tar` & `enforce_notebook_run_order-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1103 2023-06-01 21:35:18.028288 enforce_notebook_run_order-0.1.2/README.md
--rw-r--r--   0        0        0      716 2023-06-01 21:35:18.032288 enforce_notebook_run_order-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5033 2023-06-01 21:35:18.032288 enforce_notebook_run_order-0.1.2/src/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 enforce_notebook_run_order-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1103 2023-06-02 15:08:27.655664 enforce_notebook_run_order-0.1.3/README.md
+-rw-r--r--   0        0        0      716 2023-06-02 15:08:27.655664 enforce_notebook_run_order-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5033 2023-06-02 15:08:27.655664 enforce_notebook_run_order-0.1.3/src/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 enforce_notebook_run_order-0.1.3/PKG-INFO
```

### Comparing `enforce_notebook_run_order-0.1.2/README.md` & `enforce_notebook_run_order-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-0.1.2/src/enforce_notebook_run_order.py` & `enforce_notebook_run_order-0.1.3/src/enforce_notebook_run_order.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-0.1.2/PKG-INFO` & `enforce_notebook_run_order-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

