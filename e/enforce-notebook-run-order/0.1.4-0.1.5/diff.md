# Comparing `tmp/enforce_notebook_run_order-0.1.4.tar.gz` & `tmp/enforce_notebook_run_order-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enforce_notebook_run_order-0.1.4.tar", max compression
+gzip compressed data, was "enforce_notebook_run_order-0.1.5.tar", max compression
```

## Comparing `enforce_notebook_run_order-0.1.4.tar` & `enforce_notebook_run_order-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2166 2023-06-02 17:35:28.000790 enforce_notebook_run_order-0.1.4/README.md
--rw-r--r--   0        0        0      716 2023-06-02 17:35:28.000790 enforce_notebook_run_order-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5033 2023-06-02 17:35:28.000790 enforce_notebook_run_order-0.1.4/src/enforce_notebook_run_order.py
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 enforce_notebook_run_order-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2466 2023-06-02 20:03:31.754660 enforce_notebook_run_order-0.1.5/README.md
+-rw-r--r--   0        0        0      821 2023-06-02 20:03:31.758660 enforce_notebook_run_order-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5033 2023-06-02 20:03:31.758660 enforce_notebook_run_order-0.1.5/src/enforce_notebook_run_order.py
+-rw-r--r--   0        0        0     3184 1970-01-01 00:00:00.000000 enforce_notebook_run_order-0.1.5/PKG-INFO
```

### Comparing `enforce_notebook_run_order-0.1.4/README.md` & `enforce_notebook_run_order-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 This script enforces the run order of a notebook by raising an exception
 if any cells are run out of order.
 
 Usage
 -----
 
-This script can be used as a standalone script, or as a pre-commit hook.
+This script can be used as a standalone script, or as a [pre-commit
+hook](https://pre-commit.com/).
 
 ### Standalone
 
 To use `enforce-notebook-run-order` as a standalone script, simply run
 it with the path to the notebook you want to check:
 
 `enforce-notebook-run-order my_notebook.ipynb`
@@ -43,7 +44,17 @@
 
 `enforce-notebook-run-order my_notebooks/`
 
 ### Pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
+
+``` {.sourceCode .yaml}
+- repo: https://github.com/christopher-hacker/enforce-notebook-run-order
+    rev: 0.1.5
+    hooks:
+    - id: enforce-notebook-run-order
+        name: enforce-notebook-run-order
+        entry: enforce-notebook-run-order
+        types: [jupyter]
+```
```

#### html2text {}

```diff
@@ -3,14 +3,17 @@
 enforce the run order of a Jupyter notebook. Jupyter notebooks are great for
 interactive data analysis. However, when they can encourage a bad habit:
 running cells out of order. This can lead to notebooks being committed to the
 repository in a state where they don\'t run from top to bottom, and other
 collaborators may receive different results when running the notebook from top
 to bottom. This script enforces the run order of a notebook by raising an
 exception if any cells are run out of order. Usage ----- This script can be
-used as a standalone script, or as a pre-commit hook. ### Standalone To use
-`enforce-notebook-run-order` as a standalone script, simply run it with the
-path to the notebook you want to check: `enforce-notebook-run-order
-my_notebook.ipynb` Or point it to a directory to check all notebooks in that
-directory: `enforce-notebook-run-order my_notebooks/` ### Pre-commit hook To
-use `enforce_notebook_run_order` as a pre-commit hook, add the following to
-your `.pre-commit-config.yaml`:
+used as a standalone script, or as a [pre-commit hook](https://pre-commit.com/
+). ### Standalone To use `enforce-notebook-run-order` as a standalone script,
+simply run it with the path to the notebook you want to check: `enforce-
+notebook-run-order my_notebook.ipynb` Or point it to a directory to check all
+notebooks in that directory: `enforce-notebook-run-order my_notebooks/` ###
+Pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
+the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} -
+repo: https://github.com/christopher-hacker/enforce-notebook-run-order rev:
+0.1.5 hooks: - id: enforce-notebook-run-order name: enforce-notebook-run-order
+entry: enforce-notebook-run-order types: [jupyter] ```
```

### Comparing `enforce_notebook_run_order-0.1.4/src/enforce_notebook_run_order.py` & `enforce_notebook_run_order-0.1.5/src/enforce_notebook_run_order.py`

 * *Files identical despite different names*

### Comparing `enforce_notebook_run_order-0.1.4/PKG-INFO` & `enforce_notebook_run_order-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: enforce-notebook-run-order
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
+License: MIT
 Author: Chris Hacker
 Author-email: 49451910+christopher-hacker@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Project-URL: homepage, https://github.com/christopher-hacker/enforce-notebook-run-order
 Description-Content-Type: text/markdown
 
 <p align="left">
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/test.yaml">
     <img src="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/test.yaml/badge.svg" alt="Run tests">
   </a>
   <a href="https://github.com/christopher-hacker/enforce-notebook-run-order/actions/workflows/auto-tag.yml">
@@ -42,15 +45,16 @@
 
 This script enforces the run order of a notebook by raising an exception
 if any cells are run out of order.
 
 Usage
 -----
 
-This script can be used as a standalone script, or as a pre-commit hook.
+This script can be used as a standalone script, or as a [pre-commit
+hook](https://pre-commit.com/).
 
 ### Standalone
 
 To use `enforce-notebook-run-order` as a standalone script, simply run
 it with the path to the notebook you want to check:
 
 `enforce-notebook-run-order my_notebook.ipynb`
@@ -60,7 +64,17 @@
 `enforce-notebook-run-order my_notebooks/`
 
 ### Pre-commit hook
 
 To use `enforce_notebook_run_order` as a pre-commit hook, add the
 following to your `.pre-commit-config.yaml`:
 
+``` {.sourceCode .yaml}
+- repo: https://github.com/christopher-hacker/enforce-notebook-run-order
+    rev: 0.1.5
+    hooks:
+    - id: enforce-notebook-run-order
+        name: enforce-notebook-run-order
+        entry: enforce-notebook-run-order
+        types: [jupyter]
+```
+
```

#### html2text {}

```diff
@@ -1,24 +1,29 @@
-Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 0.1.4 Summary:
-Author: Chris Hacker Author-email: 49451910+christopher-
-hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: jupyter
-(>=1.0.0,<2.0.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: enforce-notebook-run-order Version: 0.1.5 Summary:
+License: MIT Author: Chris Hacker Author-email: 49451910+christopher-
+hacker@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
+(>=8.1.3,<9.0.0) Requires-Dist: jupyter (>=1.0.0,<2.0.0) Project-URL: homepage,
+https://github.com/christopher-hacker/enforce-notebook-run-order Description-
+Content-Type: text/markdown
 [Run_tests] [Create_a_tag_if_version_changed] [Publish_to_PyPi] [Build_docs]
 enforce-notebook-run-order ========================== A tiny python script to
 enforce the run order of a Jupyter notebook. Jupyter notebooks are great for
 interactive data analysis. However, when they can encourage a bad habit:
 running cells out of order. This can lead to notebooks being committed to the
 repository in a state where they don\'t run from top to bottom, and other
 collaborators may receive different results when running the notebook from top
 to bottom. This script enforces the run order of a notebook by raising an
 exception if any cells are run out of order. Usage ----- This script can be
-used as a standalone script, or as a pre-commit hook. ### Standalone To use
-`enforce-notebook-run-order` as a standalone script, simply run it with the
-path to the notebook you want to check: `enforce-notebook-run-order
-my_notebook.ipynb` Or point it to a directory to check all notebooks in that
-directory: `enforce-notebook-run-order my_notebooks/` ### Pre-commit hook To
-use `enforce_notebook_run_order` as a pre-commit hook, add the following to
-your `.pre-commit-config.yaml`:
+used as a standalone script, or as a [pre-commit hook](https://pre-commit.com/
+). ### Standalone To use `enforce-notebook-run-order` as a standalone script,
+simply run it with the path to the notebook you want to check: `enforce-
+notebook-run-order my_notebook.ipynb` Or point it to a directory to check all
+notebooks in that directory: `enforce-notebook-run-order my_notebooks/` ###
+Pre-commit hook To use `enforce_notebook_run_order` as a pre-commit hook, add
+the following to your `.pre-commit-config.yaml`: ``` {.sourceCode .yaml} -
+repo: https://github.com/christopher-hacker/enforce-notebook-run-order rev:
+0.1.5 hooks: - id: enforce-notebook-run-order name: enforce-notebook-run-order
+entry: enforce-notebook-run-order types: [jupyter] ```
```

